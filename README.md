# Kerala Doctors Register dashboard

**Live page: https://nethahussain.github.io/kerala-doctors-dashboard/**

Charts of the 67,147 doctors registered with the Travancore Cochin Medical Council (Kerala) on the
[NMC Indian Medical Register](https://nmc.org.in/information-desk/indian-medical-register/), downloaded November 2026:

- new registrations per year, by estimated gender
- how many doctors are still of working age
- doctors per 10,000 people in Kerala next to India and the world ([WHO](https://data.who.int/indicators/i/CCCEBB2/217795A))
- where Kerala's doctors studied, and foreign-trained doctors by country
- doctors by home district

Only aggregate counts are published. The tables behind each chart are in [`data/`](data/).

## Caveats

- Gender is estimated from first names (the register has no gender field); about 11% are Unknown.
- Kerala's entries on the national register stop after 2019.
- The register has no active or retired status. Working age is estimated from year of registration.
