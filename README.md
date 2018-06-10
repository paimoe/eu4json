# Europa Universalis Data
Current as of Rule Britannia.

These were parsed as part of the [EU4Map](https://github.com/paimoe/eu4map) project. Not everything is implemented yet, but the basic information is outlined below.

### countries.json
    {
      'ARA': {
        tag: "ARA",
        name: "Arakan",
        capital: 579, # provinceID
        gov: "despotic_monarchy",
        govrank: null,
        ideas: {
          ark_bengal_bay_trade: {…},
          start: {	
            light_ship_cost	"-0.20"
            num_accepted_cultures	1
          },
          trigger: {…},
          ark_muslim_advisers: {…},
          ark_rohingya_immigrants: {…},
          ark_trade_contracts_ark: {…},
          ark_magh_and_ferenghi: {…},
          free: true,
          bonus: { # ambition
            light_ship_power: "0.15",
          },
          ark_buddhist_sultans: {…},
          ark_mrauk_u_dynasty: {…}
        },
        color: "d4d397", # hex colour
        culture: "arakanese",
        religion: "theravada",
        techgroup: "chinese",
        history: [], # NotImplemented
        ideastype: "national",
        internal_name: "Arakan",
        provs: [], # provinceIDs
        cores: [1,2,3] # provinceIDs
      },
    }

### provdata.json

    {
      id: 1,
      name: "Stockholm",
      owner: "SWE",
      controller: "SWE",
      cores: ['SWE'],
      culture: "swedish",
      religion: "catholic",
      tax: 5,
      prod: 5,
      man: 3,
      trade: "grain",
      hre: false,
      claims: [],
      visible: ['eastern', 'western', 'muslim', 'ottoman'],
      sea: false,
      ocean: false,
      lake: false,
      wasteland: false,
      history: […],
      tradenode: {	
        name: "baltic_sea",
        main: false,
      },
      tile: { # Sometimes unavailable
        r: "scandinavia_region", # Region
        t: null, # Terrain (NotImplemented)
        a: "ostra_svealand_area", # Area
        c: "europe" # Continent
      }
    }

### regions.json
### tradenodes.json
### religions.json
### \_religions.json
### cultures.json
### units.json
