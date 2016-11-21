# dwp-income-support-claimants
Income Support (IS) was introduced in April 1988 can be paid to a person aged 16 to 59 who is in Great Britain, is not working 16 hours or more a week and has less money coming in than the law says they need to live on.

From October 1996, Jobseekers Allowance replaced Income Support (IS) for unemployed people. IS is now only available to people who are not required to be available for work such as carers, sick and disabled people and lone parents. The number of pensioner claimants will not equal the number of claimants aged 60 or over, as it also considers the age of the partner. Pension Credit (PC) replaced the Minimum Income Guarantee (MIG) in October 2003, PC claimants are shown separately.

Data shown here are derived from a 100% data source; the Work and Pensions Longitudinal Study (WPLS) which is not subject to any sampling error. The dataset provides counts of total claimants and breakdowns by age, gender, duration on benefit, partnering and by statistical group. Each Income Support claimant has been assigned to one of three statistical groups: Incapacity Benefits; Lone Parent; Carer or Others on Income Related Benefits. Statistical groups are arranged hierarchically and claimants are assigned to the highest statistical group that they belong to. Thus a person who claims Income Support as a Lone Parent and also receives Incapacity Benefit would be classified into incapacity benefits group. For this reason the group Lone Parent, for example will not contain all lone parents claiming Income Support. Some will be included in the Incapacity Benefits group instead. The data is a snapshot in time and will therefore exclude a small number of clerically held cases.

The snapshots are taken at quarterly intervals at the end of February (Q1), May (Q2), August (Q3) and November (Q4). The very small number of claimants who have an unknown age or gender are included within the area total but excluded from the age and gender breakdowns as they pose a small disclosure risk. The data in the WPLS datasets are not directly comparable to the annual individual level data previously released as they were a single snapshot at a point in time and did not reflect late notifications and removals from the systems. Due to the introduction of Pension Credit, rates are only shown for claimants aged 16-59, these are calculated using the population aged 16-59 from the small the area population estimates published by the National Records of Scotland. Populations denominators for higher geographies are based on best-fit 2001 geographies.

Source: Department for Work and Pensions http://statistics.gov.scot/data/income-support-claimants

## License

Data is licensed under the Open Government License: http://www.nationalarchives.gov.uk/doc/open-government-licence/version/2/

## Requirements

- NodeJS
- npm

## Installation

Clone the repository

```
git clone https://github.com/EdinburghCityScope/dwp-income-support-claimants.git
```

Install npm dependencies

```
cd dwp-income-support-claimants
npm install
```

Run the API (from the dwp-income-support-claimants directory)

```
node .
```

Converting the extracted data into loopback data.

```
node scripts/featureCollectionToLoopbackJson.js
```

Re-build data files from the statistics.gov.scot API

```
node scripts/build-data.js
```
