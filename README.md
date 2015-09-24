## Lesson Plan
1. Define `asyncio` terms and explain how generators evolved to `await`
2. Demonstrate the power of asynchronous via web client
3. Walk through javascript `EventSource` code; demonstrating async consumption
4. [Connect to server](#connect-to-server) and [Update Connection](#update-connection) via `curl`
5. [Build a Python `asyncio` Client](https://github.com/jpwatts/aioserver/blob/master/example_client3.py)
6. [Build a Python `asyncio` Server](https://github.com/jpwatts/aioserver/blob/master/aioserver/server.py)
7. Want more `asyncio` checkout out [Joel's](https://www.pytexas.org/2015/talk/50) talk
8. Connect with us on Twitter [@eloy](https://twitter.com/eloy) [@jpwatts](https://twitter.com/jpwatts)

## Connect to server
    curl "http://159.203.72.183:8000/events"

## Update Connection
    # Remember to replace the last portion with the connection id
    curl -X PUT -d '{"text":"Howdy, world"}' "http://159.203.72.183:8000/data/<replace-with-id>"