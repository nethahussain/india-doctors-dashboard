# Doctors on India's Medical Register: dashboard

**Live page: https://nethahussain.github.io/india-doctors-dashboard/**

Charts of the 1.73 million registrations on the
[NMC Indian Medical Register](https://nmc.org.in/information-desk/indian-medical-register/) (29 state councils and the
central register), downloaded November 2026. The landing page covers all of India; pick a state, or add `#KAR`, `#TC`
(Kerala), `#MAH` and so on to the address, for one council:

- a map of where doctors live, one circle per PIN code area
- each council's register, and new registrations per year by estimated gender
- how many doctors are still of working age
- doctors per 10,000 people next to the world ([WHO](https://data.who.int/indicators/i/CCCEBB2/217795A)), and state by state
- where doctors studied, and foreign-trained doctors by country
- for a state: its map, home districts, and where the council's doctors live

Only aggregate counts are published; PIN areas with fewer than five doctors are left out. The tables behind each chart
are in [`data/`](data/).

## Caveats

- Gender is estimated from first names (the register has no gender field); about 11% are Unknown India-wide.
- Several councils stopped sending entries to the national register years ago (Kerala after 2019; Bihar, Haryana and
  Madhya Pradesh after 2020). For doctors per 10,000 people, later years are projected from each council's own trend.
- The register has no active or retired status. Working age is estimated from year of registration.
- A doctor registered with two councils appears twice (about 2.4% of records), and a council's register shows where
  doctors registered, not necessarily where they work.

Map data: state boundaries from [DataMeet](https://github.com/datameet/maps) (MIT), Kerala districts from DataMeet
(CC BY 2.5 India), PIN locations from India Post's pincode directory. Populations: Government of India projections for 2026.
