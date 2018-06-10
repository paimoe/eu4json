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
    {
      'lower_don_area': {
        s: "eastern_europe_superregion",
        r: "crimea_region",
      }
    }

### tradenodes.json
    {
      'english_channel': {
        location: 1269,
        incoming: ['champagne', 'north_sea', 'chesapeake_bay', 'lubeck', 'ivory_coast'],
        members: [1269, 1270, 167, ...], # Provinces in node
        color: [220, 138, 57],
        end: true
      }
    }

### religions.json
    {
      'Christian': [
        ['Anglican', 'anglican', [135, 77, 255]],
        ['Catholic', 'catholic', [204, 204, 0]]
      ]
    }
    
### \_religions.json
Pretty much raw data from ``common/religions/00_religion.txt``

### cultures.json
    {
      Latin: ['romagnan', 'piedmontese', 'tuscan', 'ligurian', 'sardinian', 'neapolitan', 'lombard', 'venetian', 'sicilian',
        'umbrian', 'maltese'],
    }
    
### units.json
    {
      'navy': {
        'heavy_frigate': {
          type: "light_ship",
          sprite_level: 5,
          sail_speed: 10,
          hull_size: 20,
          trade_power: 4,
          base_cannons: 25
        }
      },
      'army': {
        'bhonsle_infantry	': {
          'stats': {
            om: 2, # Offensive Morale
            of: 3 # Offensive Fire
            os: 2, # Offensive Shock
            m: 1, # Maneuver
            dm: 2, # Defensive Morale
            ds: 2, # Defensive Shock
            df: 3 # Defensive Fire
          },
          type: 'infantry',
          unit_type: 'indian',
        }
      }
    }
