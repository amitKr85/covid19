# covid19
analysis of confirm, death, recovered cases of covid-19 

# data taken from https://github.com/CSSEGISandData/COVID-19

# json data available in json/ with file name as covid19_{month}_{date}_{year}.json containing data till month-date-year
format of json is: 
{
	"GLOBAL":{
			"Cumulative":{
					"Confirmed": x, "Deaths": y, "Recovered": z
				},
			"1-22-2020":{
					"Cumulative":{
						"Confirmed": x, "Deaths": y, "Recovered": z
					},
					"Current":{
						"Confirmed": x, "Deaths": y, "Recovered": z
					}
				},
			"1-23-2020":{
					...
				},
				...
		},
	"Country1":{
			...
		},
	"Country2":{
			...
	},
	...

}

where,
GLOBAL contains Global data.
Country1, Country2 are Country names containing country data related to covid19.
Cumulative Key under Country contains total confirmed, deaths, recovered cases till month-date-year
Each date contains date specific data.
Current key under specific-date contains increment in number of confirmed, deaths, recovered cases from previous day.
Cumulative key under specific-date contains total number of confirmed, deaths, recovered cases till the date.



