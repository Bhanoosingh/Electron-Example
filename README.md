```
1. npm init(for project configration)
    1. add in scripts "start": "electron index.js"
	2. add this code on index.js file
		const electron=require('electron')
		const {app,BrowserWindow}=electron

		app.on('ready',()=>{
    			let win=new BrowserWindow({width:800,height:800, 
        			webPreferences: {
                			nodeIntegration: true
        			}
    			})
    			win.loadURL(`file://${__dirname}/index.html`)
		})

	3. add index.html and page2.html(for multiple page)

```	
---
```
2. npm i electron --save-dev
```
---
```
3. npm i electron-reload --save-dev(to render application without relod)
```
---
```
4. npm start(To run app)
```
---