# nordpool-growatt
A Nordpool chart and table for growatt inverters with solax modbus hacs integration.  In addition to a chart (copied from ha forum) it will show a price table with grid/battery periods colored 

The Nordpool chart requires the core Nordpool integration and Apexcharts. 
The chart is taken completely from Home Assistant forum from a member
Teebar I think, from this link

https://community.home-assistant.io/t/tomorrows-price-unavailable-with-nordpool-core-integration/838167/11

The table is almost all up to chatgpt. It uses the Solax modbus hacs integration
here https://github.com/wills106/homeassistant-solax-modbus
It uses the prefix growatt_inverter for its entities. If you use something else 
search and replace. 

I know the html has some syntax errors, but it works (double ending
font tags). I didn't know how to avoid them and thought one extra is
better than one missing. Chatgpt didn't know either, except for
km lengths of code that eventually maybe could have worked.

To install it you need to include or copy a file into your 
configuration.yaml file and create a manual card in ha and
paste the yaml code into it.

Then you need to create a helper in HA Settings->Helper (2nd from top usually)
and click on Helper and click Create helpe and select Input boolean and name it
'show_table'

Mikael Wahlgren
