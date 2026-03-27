# WingWeave

A garden planning tool designed to help people support local butterfly and moth populations through intentional planting.

## Project Vision

Most pollinator gardening advice focuses on planting nectar flowers. WingWeave goes further by helping gardeners support the full life cycle of butterflies and moths.

The goal is to connect:

- butterfly and moth species  
- to their host plants for egg laying  
- to larval food sources  
- to nectar plants for adults  

This allows gardeners to move beyond general pollinator support and build gardens that function as real habitat.

## Core Concept

Gardeners plant with three goals:

1. Host plants for egg laying  
2. Larval food sources (caterpillars)  
3. Adult nectar sources  

The tool connects these relationships to specific species found in the user’s region.
## Dataset (Phase 1)

The initial dataset includes:

- ~10 butterfly species relevant to Alberta (Zone 3)
- 20–30 plant species
- Relationships categorized as:
  - larval (host plants)
  - nectar (adult feeding)
- Scientific names for plants and insects
- Source type and confidence level for each entry

This dataset is designed to be "good enough" to support a working prototype and will be refined over time.
## Next Steps (Phase 2)

- Build a simple lookup tool using Python and pandas
- Allow filtering by:
  - butterfly species
  - ecological role (larval vs nectar)
  - growing conditions (e.g., sun exposure)
- Generate plant recommendations based on user input
Phase 2: Prototype Development
In Phase 2, WingWeave was developed into a functional Python-based prototype using Jupyter Notebook and pandas.
The goal of this phase was to move beyond static data and demonstrate how the dataset can be used to generate meaningful, actionable recommendations for gardeners.
Key Features Implemented
•	Species-based querying 
o	Users can input a butterfly species to receive relevant planting recommendations 
•	Plant role separation 
o	Distinguishes between: 
	Host plants (for egg-laying and larval development) 
	Nectar plants (for adult nourishment) 
•	Environmental filtering 
o	Supports filtering by: 
	Sun exposure (e.g., Full sun) 
	Plant growth habit (e.g., Herbaceous, Tree, Shrub) 
•	Dual output modes 
o	full mode: displays all relevant host and nectar plants 
o	starter mode: generates a simplified planting plan: 
	1–2 host plants 
	2–3 nectar plants
•	Human-readable output 
o	Results formatted for clarity and usability 
o	Includes both common and botanical plant names 
Example Use Case
A user can query:
get_garden_plan("Monarch", sun="Full", growth="Herbaceous", mode="starter")
And receive a structured garden plan tailored to both ecological function and growing conditions.
________________________________________
What This Demonstrates
This phase demonstrates the ability to:
•	Translate ecological relationships into structured data models 
•	Build reusable logic using Python and pandas 
•	Design a decision-support tool based on real-world constraints 
•	Balance scientific accuracy with practical usability 
________________________________________
Phase 3: Next Steps
Phase 3 will focus on improving usability and accessibility by introducing a more intuitive user experience.
Planned enhancements include:
•	Menu-driven input flow
o	Allow users to select butterflies, sun conditions, and growth habit preferences without writing code
•	Streamlit-based interface
o	Transform the notebook prototype into a simple web app
o	Enable interactive selection and real-time recommendations
•	Improved output formatting
o	More structured and visual presentation of garden plans
Status
Phase 2 is complete. The WingWeave prototype is now capable of generating meaningful, customizable planting recommendations based on butterfly species and environmental conditions.
