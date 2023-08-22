# CumulusCI Notes

### Connects devhub with cci
`cci service connect devhub <devHubAlias>` 

### Creates a scratch org, the alias < > should match the one in the cumulusci.yml
`cci org info <dev_2>`

### Push the existing metadata to your dev org
`cci flow run dev_org --org <dev_2>`

### Open dev org in the browser
`cci org browser <dev_2>`

### Retrieve changes in your org
`cci task run retrieve_changes --org <dev_2>`

### Documentation on scratch org creation 
[https://cumulusci.readthedocs.io/en/stable/scratch-orgs.html](https://cumulusci.readthedocs.io/en/stable/scratch-orgs.html)

# Snowfakery Notes

### Generate and load data from a Snowfakery recipe
`cci task run snowfakery --recipe snowfakeryData/Account.recipe.yml --run-until-recipe-repeated 300 --org dev_2`