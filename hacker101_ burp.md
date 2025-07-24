hacker101: burp

burp 101: getting started

* proxy -> options shows what port the proxy is on
* set proxy in firefox (foxyproxy!)
* install burp cert:
	* http://burp
	* ff options -> privacy -> security to install into cert manager
* hit intercept tab, turn off. page should load
* tabs:
	* target = tree of sites, plus set scope
	* proxy = intrerceptor, htp history, websockets history, and options galore
	* spider = can find stuff you missed
	* scanner = (pro only)
	* intruder = make multiple requests with payloads
	* repeater = repeat existing requests to test for bugs
	* sequencer - intercept tokens and inspect
	* decoder - decode hex, base64, etc
	* compare - compare 2 blocks of data
* target!
	* site map shows pages you have accessed. links in grey mean that spider found a ref but no request hit it (bad link, unknown functionality.)
	* This is where you can set scope (right click, add to scope)
* proxy
	* history is about 50% of your time in burp
		* you can filter to whats in scope
	* match and replace function. you can change anything from running JS to refering agent
* intercept
	* catches data, allows you to change, and submit
	* you may not be seeing a bug, what you see only effects your browser
* repeater
	* execute requests and see the response

burp 201: maximizing burp
* most of this is pro only. a rank of 500+ and positive trend on hacker1 will get you a 3 month discount
* intruder:
	* positions: set type of attack
	* payloads: set payload set and type
	* options: grep extract
* scanner:
	* can do passive and active
		* passive runs on everything (in or out of scope) while you work
		* active is a targeted scan on just your scope. best to send to active from proxy history
		* issue activity is your history
* burp otions -> search allows search across all your project!
	* in history: r click, engagement tools -> generate csrf poc

burp 301: burp hacks for bounty hunters

* repeater (manual scan/manual check)
	* name your tabs
	* use the forward and back button to prevent 1000s of tabs
	* use the search and sutoscroll
	* dont forget domain fronting (send to one while showing you are sending to anther)
	* streaming responses
* intruder (automatic scan/manual check)
	* use your own wordlists!
	* grep extract is life
	* scan check builder: easily build scan checks (automate the manual checks)
	* 
* scanner
* performance and problem solving
* q&a