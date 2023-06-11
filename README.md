# geolocation
A sample Salesforce DX App

[Trailhead exercise](https://trailhead.salesforce.com/content/learn/modules/sfdx_app_dev/sfdx_app_dev_create_app)


## Create the project.

```
sf force:project:create -n geolocation
```

```
cd geolocation
```

```
sf force:org:create -s -f config/project-scratch-def.json -a GeoAppScratch
```


## Create Sample Data

Create the Marriott Marquis account
```
sfdx force:data:record:create -s Account -v "Name='Marriott Marquis' BillingStreet='780 Mission St' BillingCity='San Francisco' BillingState='CA' BillingPostalCode='94103' Phone='(415) 896-1600' Website='www.marriott.com'"
```

Create the Hilton Union Square account.
```
sfdx force:data:record:create -s Account -v "Name='Hilton Union Square' BillingStreet='333 O Farrell St' BillingCity='San Francisco' BillingState='CA' BillingPostalCode='94102' Phone='(415) 771-1400' Website='www.hilton.com'"
```

Create the Hyatt account.
```
sfdx force:data:record:create -s Account -v "Name='Hyatt' BillingStreet='5 Embarcadero Center' BillingCity='San Francisco' BillingState='CA' BillingPostalCode='94111' Phone='(415) 788-1234' Website='www.hyatt.com'"
```
