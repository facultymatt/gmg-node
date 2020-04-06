
# Overview

The point is a useful webapp for visualizing and tracking Green Mountain Grill cooks. This is a proof of concept which uses the work from https://github.com/Aenima4six2/gmg to decode the grill status which is sent over UDP when the grill gets the right command. This code aims to be much simplier to reason than Aenima4six2/gmg, and easier to get running and customize. 

This spike write data to a CSV as a database (which proved to be more trouble than worth) and visualizes prob1 temp using a ascii line chart. Another command prompt can run a real-time dashboard, although its very buggy due to reading / writing to files. 

To get started 

- Install deps `npm install`
- Configure for your grill in `./config.js`
- Run `npm run start`
- Additionally, in a new command window, run `npm run dashboard`
- See CSV generated in `./data` folder

# Next steps

- Use a real database to sync data from server to client
- Test and reafactor the GrillStatus class
- Add react front-end with proper graphs.
- Try sending commands? 
- Debug profiles and what they are all about - do we need them if we can set a profile on this? 




# Useful links

- https://community.hubitat.com/t/release-green-mountain-grill/34720


# Charting libs

- https://github.com/yaronn/blessed-contrib

