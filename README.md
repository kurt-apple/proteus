# Proteus
My everything data dashboard
## Purpose
I use Airtable obsessively. I have dozens of bases, each with dozens of tables. As my data grows, my need for advanced funtionality grows too. Some examples of features Airtable currently lacks are:
- raw sql query
- foreach
- select item.name where item.attribute meets condition (for instance, finding the name of MAX(values))
- array functions
- client-side calculations (possible to cache data somehow?)
I aim to solve this by pulling the data, running calculations on my side, and then pushing data back up. If I run in to hurdles... well... I will continue to evolve Proteus to fit my needs.
## Stack
### Data is stored in Airtable.
This project uses Airtable as the data store. This is tremendously useful as the overall schema can change often, and the Proteus features I intend to build are all things that are time-sensitive. As a one-person operation, I can't manage a data server right now.
### Frontend is built with Quasar.
Quasar builds upon Vue. It's another helpful time-saving tool.
### Deployed with a Docker container.
I will containerize this app in order to speed up deployment and hopefully transition to CI/CD in the near future. I think having a robust testing apparatus will be extremely important.
## Stretch Goals
I don't want to limit this platform to the Airtable API. I would really like to eventually pull in data from a finance API in order to create trading data dashboards. To do so, I will need a way to form API connectors in-app. Currently, this is defined in connection.json.
Also, in the future, I would really like to use my own database. But again, that is too time-consuming right now. Gotta get my feet wet first.
