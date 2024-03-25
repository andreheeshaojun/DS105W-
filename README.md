## About me

I am a student at the _LSE_ studying BSc Economics.

I will use this GitHub profile to showcase my data science skills.

### Interests

- Python 
- Data Science


 ```mermaid
graph LR
    A("Machine Mavericks") 
    B("Data Collection")
    C("Data Cleaning & Pre-Processing")
    D("Combination & Extrapolation")
    E("Data Analysis")
    F("Data Visualisation")

    A --> B
    B --> C
    C --> D
    D --> E
    E --> F

    G("i. Waitrose Products")
    H("ii. Ultra-Processed Food")

    B --> G
    B --> H

    I("Meat")
    J("Carbohydrates")
    K("Vegetables")

    G --> I
    G --> J
    G --> K

    L("https://www.waitrose.com/ecom/shop/browse/groceries/fresh_and_chilled/fresh_vegetables")
    M("https://www.waitrose.com/ecom/shop/browse/groceries/fresh_and_chilled/fresh_meat")
    N("https://www.waitrose.com/ecom/shop/browse/groceries/food_cupboard/rice_pasta_and_pulses")

    I --> |"Using CSS and XPath Selectors; Webscraping"| M
    J --> |"Using CSS and XPath Selectors; Webscraping"| N
    K --> |"Using CSS and XPath Selectors; Webscraping"| L

    O("Waitrose")

    L --> |"Send Get Request"| O
    M --> |"Send Get Request"| O
    N --> |"Send Get Request"| O

    P("Price/100g, Nutrients/100g, Shelf Life")

    O --> |"Scrape for"| P

    Q("Harvard")
    R("Canadian Institute of Intestinal Research")
    S("British Heart Foundation")

    H --> Q
    H --> R
    H --> S

    T("Dataframe for Ultra-Processed Food")

    Q --> T
    R --> |"Filtering for most commonly stated ultra-processed food"| T
    S --> T

    U("Cleaning ultra-processed food data")
    V("Removing abnormalities for standardisation")

    C --> U
    U --> V

    W("Cleaning raw data from Waitrose")

    C --> W

    X("Remove 'per serving' ingredients")
    Y("Convert per kg to per g")
    Z("Exclude ingredients without nutritional value")
    AA("Only keep desired columns")
    AD("Remove ultra processed ingredients")
    AF("Obtain merged dataframe between Waitrose and ultra-processed foods")

    W --> X
    W --> Y
    W --> Z
    W --> AA
    W --> AD
    AD --> AF
    T -->|Used to| AD

    AB("Name, Price per unit, Energy, Protein, Fat, Saturated Fat, Carbohydrate, Sugar, Fibre, Salt, Shelf life")

    AA --> AB

    AC("Obtain Top 20 in each category")

    AF --> |"Used In"| D
    D --> |"Based on customer reviews"| AC

    AE("Find out 8,000 prospective combinations of food")

    AC --> AE
    AE --> |"Used In"| E

    AG("Aggregate nutritional value")
    AH("Calculate total price/100g")
    AI("Sensitivity for respective budget threshold")
    AJ("Regression Analysis")
    AK("Combo vs shelf life")
    AL("Sensitivity Test")

    E --> AG
    AG --> AH
    AH --> AI
    E --> |"Taking minimum bundle shelf life"| AJ
    AJ --> AK
    E --> AL

