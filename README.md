# linkedin-personal-network-visualization


## Inspiration
Throughout a Seminar at Technical University for Data Mining for Social Networks I developed this code to visualize my own personal network and lay a basis for personal network visualization.

## What it does
linkedin-network-visualization takes your [exported connections data from LinkedIn](https://www.linkedin.com/help/linkedin/answer/66844/export-connections-from-linkedin) and render it into a node graph.

With the visualization, you can identify the companies where the majority of your connections are working to reach out for job opportunities, as well as those hidden small companies you never thought of. The cut-off for companies is a minimum of 3 connections of your own community.

Afterwards you can search for names and look for specific people in the graph.

## How I built it
The `connections.csv` file from LinkedIn is parsed in to an object and then rendered with [D3.js v4 Force Directed Graph with Labels](https://bl.ocks.org/heybignick/3faf257bbbbc7743bb72310d03b86ee8)

The nodes of the graph are generated from your connections.
The edges of the graph are generated for connections who work at the same company.

## Challenges

The main reason I decided for this way of portraying the network only with the connections.csv file is that LinkedIn is very restrictive about the usage of the API and also custom API's or webscrapers don't work that well and may result in an account ban.

## Outlook

If there are any new possibilities to enhance the code and add further degrees of connections and enrich the data, feel free to collaborate with me on this code. See this as a basis for an own analysis tool of your network.

## References
[linkedin_api](https://github.com/tomquirk/linkedin-api)

[linkedin-network-visualization](https://github.com/Thanh-To/linkedin-network-visualization)

[D3.js v4 Force Directed Graph with Labels](https://bl.ocks.org/heybignick/3faf257bbbbc7743bb72310d03b86ee8)
