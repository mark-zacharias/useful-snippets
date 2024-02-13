run the following to create a tunnel then host it.  If you just host a tunnel it gets deleted when you stop the process.  Creating it first allows you to keep the same url each time you start it up.
 
`devtunnel user login`
`devtunnel create -a -d core` to create an anon tunnel with the description 'core'
`devtunnel port create -p 44305 --protocol https` to add the https port to connect to
`devtunnel host` to host the tunnel.


use the output url to update your .env file.
you can close this tunnel and subsquent times just run `devtunnel host` to open the same tunnel.
if you don't use it for 30 days it'll be deleted.
