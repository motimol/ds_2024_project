MSSubClass: Identifies the type of dwelling involved in the sale.	
# Categorical - OHE

        20	1-STORY 1946 & NEWER ALL STYLES
        30	1-STORY 1945 & OLDER
        40	1-STORY W/FINISHED ATTIC ALL AGES
        45	1-1/2 STORY - UNFINISHED ALL AGES
        50	1-1/2 STORY FINISHED ALL AGES
        60	2-STORY 1946 & NEWER
        70	2-STORY 1945 & OLDER
        75	2-1/2 STORY ALL AGES
        80	SPLIT OR MULTI-LEVEL
        85	SPLIT FOYER
        90	DUPLEX - ALL STYLES AND AGES
       120	1-STORY PUD (Planned Unit Development) - 1946 & NEWER
       150	1-1/2 STORY PUD - ALL AGES
       160	2-STORY PUD - 1946 & NEWER
       180	PUD - MULTILEVEL - INCL SPLIT LEV/FOYER
       190	2 FAMILY CONVERSION - ALL STYLES AND AGES

MSZoning: Identifies the general zoning classification of the sale.
# Categorical - OHE
		
       A	Agriculture
       C	Commercial
       FV	Floating Village Residential
       I	Industrial
       RH	Residential High Density
       RL	Residential Low Density
       RP	Residential Low Density Park 
       RM	Residential Medium Density
	
LotFrontage: Linear feet of street connected to property

LotArea: Lot size in square feet

Street: Type of road access to property
# binary (1 - paved, 0 - gravel)

       Grvl	Gravel	
       Pave	Paved
       	
Alley: Type of alley access to property
# null - "no alley"
# Categorical - OHE
# *PERHAPS* ordinal

       Grvl	Gravel
       Pave	Paved
       NA 	No alley access
		
LotShape: General shape of property
# "irregularity": ordinal. 0(regular) -> 3 (Irregular)

       Reg	Regular	
       IR1	Slightly irregular
       IR2	Moderately Irregular
       IR3	Irregular
       
LandContour: Flatness of the property
# "flatness". ordinal. 0 depression-> 3 lvl

       Lvl	Near Flat/Level	
       Bnk	Banked - Quick and significant rise from street grade to building
       HLS	Hillside - Significant slope from side to side
       Low	Depression
		
Utilities: Type of utilities available
# "Utility": ordinal. 0(ELO) -> 3 (AllPub)
		
       AllPub	All public Utilities (E,G,W,& S)	
       NoSewr	Electricity, Gas, and Water (Septic Tank)
       NoSeWa	Electricity and Gas Only
       ELO	Electricity only	
	
LotConfig: Lot configuration
# Categorical - OHE

       Inside	Inside lot
       Corner	Corner lot
       CulDSac	Cul-de-sac
       FR2	Frontage on 2 sides of property
       FR3	Frontage on 3 sides of property
	
LandSlope: Slope of property
# "irregularity": ordinal. 0(regular) -> 3 (Irregular)
		
       Gtl	Gentle slope
       Mod	Moderate Slope	
       Sev	Severe Slope
	
Neighborhood: Physical locations within Ames city limits
# Categorical - OHE

       Blmngtn	Bloomington Heights
       Blueste	Bluestem
       BrDale	Briardale
       BrkSide	Brookside
       ClearCr	Clear Creek
       CollgCr	College Creek
       Crawfor	Crawford
       Edwards	Edwards
       Gilbert	Gilbert
       IDOTRR	Iowa DOT and Rail Road
       MeadowV	Meadow Village
       Mitchel	Mitchell
       Names	North Ames
       NoRidge	Northridge
       NPkVill	Northpark Villa
       NridgHt	Northridge Heights
       NWAmes	Northwest Ames
       OldTown	Old Town
       SWISU	South & West of Iowa State University
       Sawyer	Sawyer
       SawyerW	Sawyer West
       Somerst	Somerset
       StoneBr	Stone Brook
       Timber	Timberland
       Veenker	Veenker
			
Condition1: Proximity to various conditions
# Categorical - 2 OHE -> OR between them 
	
       Artery	Adjacent to arterial street
       Feedr	Adjacent to feeder street	
       Norm	Normal	
       RRNn	Within 200' of North-South Railroad
       RRAn	Adjacent to North-South Railroad
       PosN	Near positive off-site feature--park, greenbelt, etc.
       PosA	Adjacent to postive off-site feature
       RRNe	Within 200' of East-West Railroad
       RRAe	Adjacent to East-West Railroad
	
+ Condition2: Proximity to various conditions (if more than one is present)
		
       Artery	Adjacent to arterial street
       Feedr	Adjacent to feeder street	
       Norm	Normal	
       RRNn	Within 200' of North-South Railroad
       RRAn	Adjacent to North-South Railroad
       PosN	Near positive off-site feature--park, greenbelt, etc.
       PosA	Adjacent to postive off-site feature
       RRNe	Within 200' of East-West Railroad
       RRAe	Adjacent to East-West Railroad
	
BldgType: Type of dwelling
# Categorical - OHE
		
       1Fam	Single-family Detached	
       2FmCon	Two-family Conversion; originally built as one-family dwelling
       Duplx	Duplex
       TwnhsE	Townhouse End Unit
       TwnhsI	Townhouse Inside Unit
	
HouseStyle: Style of dwelling
	
       1Story	One story - 1
       1.5Fin	One and one-half story: 2nd level finished - 1.5
       1.5Unf	One and one-half story: 2nd level unfinished - 1.25
       2Story	Two story - 2
       2.5Fin	Two and one-half story: 2nd level finished 2.5
       2.5Unf	Two and one-half story: 2nd level unfinished 2.25
       SFoyer	Split Foyer 3
       SLvl	Split Level 3.5
	
OverallQual: Rates the overall material and finish of the house
# no action
       10	Very Excellent
       9	Excellent
       8	Very Good
       7	Good
       6	Above Average
       5	Average
       4	Below Average
       3	Fair
       2	Poor
       1	Very Poor
	
OverallCond: Rates the overall condition of the house
# no action
       10	Very Excellent
       9	Excellent
       8	Very Good
       7	Good
       6	Above Average	
       5	Average
       4	Below Average	
       3	Fair
       2	Poor
       1	Very Poor
		
YearBuilt: Original construction date
# no action

YearRemodAdd: Remodel date (same as construction date if no remodeling or additions)
# no action

RoofStyle: Type of roof
# Categorical - OHE
       Flat	Flat
       Gable	Gable
       Gambrel	Gabrel (Barn)
       Hip	Hip
       Mansard	Mansard
       Shed	Shed
		
RoofMatl: Roof material
# Categorical - OHE
       ClyTile	Clay or Tile
       CompShg	Standard (Composite) Shingle
       Membran	Membrane
       Metal	Metal
       Roll	Roll
       Tar&Grv	Gravel & Tar
       WdShake	Wood Shakes
       WdShngl	Wood Shingles
		
Exterior1st: Exterior covering on house
# Categorical - 2 OHE -> OR between them 
       AsbShng	Asbestos Shingles
       AsphShn	Asphalt Shingles
       BrkComm	Brick Common
       BrkFace	Brick Face
       CBlock	Cinder Block
       CemntBd	Cement Board
       HdBoard	Hard Board
       ImStucc	Imitation Stucco
       MetalSd	Metal Siding
       Other	Other
       Plywood	Plywood
       PreCast	PreCast	
       Stone	Stone
       Stucco	Stucco
       VinylSd	Vinyl Siding
       Wd Sdng	Wood Siding
       WdShing	Wood Shingles
	
Exterior2nd: Exterior covering on house (if more than one material)

       AsbShng	Asbestos Shingles
       AsphShn	Asphalt Shingles
       BrkComm	Brick Common
       BrkFace	Brick Face
       CBlock	Cinder Block
       CemntBd	Cement Board
       HdBoard	Hard Board
       ImStucc	Imitation Stucco
       MetalSd	Metal Siding
       Other	Other
       Plywood	Plywood
       PreCast	PreCast
       Stone	Stone
       Stucco	Stucco
       VinylSd	Vinyl Siding
       Wd Sdng	Wood Siding
       WdShing	Wood Shingles
	
MasVnrType: Masonry veneer type
# Categorical - OHE
       BrkCmn	Brick Common
       BrkFace	Brick Face
       CBlock	Cinder Block
       None	None
       Stone	Stone
	
MasVnrArea: Masonry veneer area in square feet
# no action

ExterQual: Evaluates the quality of the material on the exterior 
		
       Ex	Excellent -5
       Gd	Good-4
       TA	Average/Typical-3
       Fa	Fair 2
       Po	Poor 1
		
ExterCond: Evaluates the present condition of the material on the exterior
		
       Ex	Excellent -5
       Gd	Good-4
       TA	Average/Typical-3
       Fa	Fair 2
       Po	Poor 1
		
Foundation: Type of foundation
# OHE
       BrkTil	Brick & Tile
       CBlock	Cinder Block
       PConc	Poured Contrete	
       Slab	Slab
       Stone	Stone
       Wood	Wood
		
BsmtQual: Evaluates the height of the basement

       Ex	Excellent (100+ inches)	5
       Gd	Good (90-99 inches) 4
       TA	Typical (80-89 inches) 3
       Fa	Fair (70-79 inches)2
       Po	Poor (<70 inches 1
       NA	No Basement 0
		
BsmtCond: Evaluates the general condition of the basement

       Ex	Excellent 5
       Gd	Good 4
       TA	Typical - slight dampness allowed 3
       Fa	Fair - dampness or some cracking or settling 2
       Po	Poor - Severe cracking, settling, or wetness 1
       NA	No Basement 0
	
BsmtExposure: Refers to walkout or garden level walls
# Check if removing entries that do not have a basement and a positive exposure (1<)

       Gd	Good Exposure 4
       Av	Average Exposure (split levels or foyers typically score average or above)	3
       Mn	Mimimum Exposure 2
       No	No Exposure 1
       NA	No Basement 0
	
BsmtFinType1: Rating of basement finished area
# OHE + OR

       GLQ	Good Living Quarters 6
       ALQ	Average Living Quarters
       BLQ	Below Average Living Quarters	
       Rec	Average Rec Room
       LwQ	Low Quality
       Unf	Unfinshed 
       NA	No Basement 0
		
BsmtFinSF1: Type 1 finished square feet
# no action

BsmtFinType2: Rating of basement finished area (if multiple types)

       GLQ	Good Living Quarters
       ALQ	Average Living Quarters
       BLQ	Below Average Living Quarters	
       Rec	Average Rec Room
       LwQ	Low Quality
       Unf	Unfinshed
       NA	No Basement

BsmtFinSF2: Type 2 finished square feet
# no action

BsmtUnfSF: Unfinished square feet of basement area
# no action

TotalBsmtSF: Total square feet of basement area
# no action

Heating: Type of heating
# OHE		
       Floor	Floor Furnace
       GasA	Gas forced warm air furnace
       GasW	Gas hot water or steam heat
       Grav	Gravity furnace	
       OthW	Hot water or steam heat other than gas
       Wall	Wall furnace
		
HeatingQC: Heating quality and condition

       Ex	Excellent 5
       Gd	Good 4
       TA	Average/Typical 3
       Fa	Fair 2
       Po	Poor 1
		
CentralAir: Central air conditioning
# To numerical
       N	No 0
       Y	Yes 1
		
Electrical: Electrical system
# OHE
       SBrkr	Standard Circuit Breakers & Romex
       FuseA	Fuse Box over 60 AMP and all Romex wiring (Average)	
       FuseF	60 AMP Fuse Box and mostly Romex wiring (Fair)
       FuseP	60 AMP Fuse Box and mostly knob & tube wiring (poor)
       Mix	Mixed
	#Blanks: "Blank"
		
1stFlrSF: First Floor square feet
# no action
 
2ndFlrSF: Second floor square feet
# no action

LowQualFinSF: Low quality finished square feet (all floors)
# no action

GrLivArea: Above grade (ground) living area square feet
# no action

BsmtFullBath: Basement full bathrooms
# no action

BsmtHalfBath: Basement half bathrooms
# no action

FullBath: Full bathrooms above grade
# no action

HalfBath: Half baths above grade
# no action

Bedroom: Bedrooms above grade (does NOT include basement bedrooms)
# no action

Kitchen: Kitchens above grade
# no action

KitchenQual: Kitchen quality

       Ex	Excellent 5
       Gd	Good 4
       TA	Typical/Average 3
       Fa	Fair 2
       Po	Poor 1
       	
TotRmsAbvGrd: Total rooms above grade (does not include bathrooms)
# no action

Functional: Home functionality (Assume typical unless deductions are warranted)

       Typ	Typical Functionality - 8
       Min1	Minor Deductions 1
       Min2	Minor Deductions 2
       Mod	Moderate Deductions
       Maj1	Major Deductions 1
       Maj2	Major Deductions 2
       Sev	Severely Damaged
       Sal	Salvage only - 1
		
Fireplaces: Number of fireplaces
# no action

FireplaceQu: Fireplace quality

       Ex	Excellent - Exceptional Masonry Fireplace - 5
       Gd	Good - Masonry Fireplace in main level
       TA	Average - Prefabricated Fireplace in main living area or Masonry Fireplace in basement
       Fa	Fair - Prefabricated Fireplace in basement
       Po	Poor - Ben Franklin Stove
       NA	No Fireplace - 0
		
GarageType: Garage location
# OHE		
       2Types	More than one type of garage
       Attchd	Attached to home
       Basment	Basement Garage
       BuiltIn	Built-In (Garage part of house - typically has room above garage)
       CarPort	Car Port
       Detchd	Detached from home
       NA	No Garage
		
GarageYrBlt: Year garage was built
# no action
		
GarageFinish: Interior finish of the garage

       Fin	Finished - 3
       RFn	Rough Finished	
       Unf	Unfinished
       NA	No Garage - 0
		
GarageCars: Size of garage in car capacity
# no action

GarageArea: Size of garage in square feet
# no action

GarageQual: Garage quality

       Ex	Excellent - 5
       Gd	Good
       TA	Typical/Average
       Fa	Fair
       Po	Poor
       NA	No Garage - 0
		
GarageCond: Garage condition

       Ex	Excellent - 5
       Gd	Good
       TA	Typical/Average
       Fa	Fair
       Po	Poor
       Blanks	No Garage - 0
		
PavedDrive: Paved driveway

       Y	Paved - 2
       P	Partial Pavement - 1
       N	Dirt/Gravel - 0
		
WoodDeckSF: Wood deck area in square feet
# no action

OpenPorchSF: Open porch area in square feet
# no action

EnclosedPorch: Enclosed porch area in square feet
# no action

3SsnPorch: Three season porch area in square feet
# no action

ScreenPorch: Screen porch area in square feet
# no action

PoolArea: Pool area in square feet
# no action

PoolQC: Pool quality
		
       Ex	Excellent -4
       Gd	Good
       TA	Average/Typical
       Fa	Fair
       NA	No Pool - 0
		
Fence: Fence quality
# OHE		
       GdPrv	Good Privacy
       MnPrv	Minimum Privacy
       GdWo	Good Wood
       MnWw	Minimum Wood/Wire
       NA	No Fence
	
MiscFeature: Miscellaneous feature not covered in other categories
# OHE		
       Elev	Elevator
       Gar2	2nd Garage (if not described in garage section)
       Othr	Other
       Shed	Shed (over 100 SF)
       TenC	Tennis Court
       NA	None
		
MiscVal: $Value of miscellaneous feature
# no action

MoSold: Month Sold (MM)
# no action

YrSold: Year Sold (YYYY)
# no action

SaleType: Type of sale
# OHE		
       WD 	Warranty Deed - Conventional
       CWD	Warranty Deed - Cash
       VWD	Warranty Deed - VA Loan
       New	Home just constructed and sold
       COD	Court Officer Deed/Estate
       Con	Contract 15% Down payment regular terms
       ConLw	Contract Low Down payment and low interest
       ConLI	Contract Low Interest
       ConLD	Contract Low Down
       Oth	Other
		
SaleCondition: Condition of sale
# OHE
       Normal	Normal Sale
       Abnorml	Abnormal Sale -  trade, foreclosure, short sale
       AdjLand	Adjoining Land Purchase
       Alloca	Allocation - two linked properties with separate deeds, typically condo with a garage unit	
       Family	Sale between family members
       Partial	Home was not completed when last assessed (associated with New Homes)
