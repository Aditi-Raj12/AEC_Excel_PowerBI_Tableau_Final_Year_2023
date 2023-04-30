# AEC_Excel_PowerBI_Tableau_Final_Year_2023

**GitHub Link:**<br>
https://github.com/toarnabtrainer/AEC_Excel_PowerBI_Tableau_Final_Year_2023<br>
or<br>
https://tinyurl.com/2bwuyu5v<br>

**GMeet Link:**<br>
https://meet.google.com/ugx-iskt-vbc

**Online Session MS-Teams Link for all sessions:**<br>
https://tinyurl.com/y8hmh8bt

**PowerBI Download Link:**<br>
https://www.microsoft.com/en-us/download/details.aspx?id=58494

**PDF Link on the Cloud:**<br>
https://www.indiapost.gov.in/VAS/DOP_PDFFiles/Civillistnew.pdf

**Web Portal Link:**<br>
https://www.contextures.com/xlsampledata01.html

**Create your free account on Tableau:**<br>
https://www.tableau.com/<br>
https://public.tableau.com/app/discover

**Tutorial and Official Documentation on MS-Power BI Link:**<br>
https://docs.microsoft.com/en-us/power-bi/desktop-create-and-manage-relationships

**Lookup and Dimension Tables**<br>
Lookup Tables or Dimension Tables will have Primary Keys, will answer Who, What, Where, When and How<br>
Data Tables or Fact Table will have Foreign Keys, and will contain transactional data

**Data Relationships for the Budget Project**<br>
* Sales(CustomerKey) -> Customer(CustomerKey)<br>
* Sales(OrderDate) -> Calendar(Date)<br>
* Sales(ProductKey) -> Product(ProductKey)<br>
* Sales(SalesTerritoryKey) -> Territories(SalesTerritoryKey)<br>
* Budget(ProdyctKey) -> Product(ProductKey)<br>
* Budget(Month) -> Calendar(Date)<br>

**DAX Functions:**<br>
TotalSales = SUM(RN_East1[EastSales])  // SUM(Coolumn Name)<br>
AverageSales = AVERAGE(RN_East1[EastSales])  // AVERAGE(Column Name)<br>
CountSales = COUNT(RN_East1[EastSales])   // COUNT(Column Name)<br>
MaxSales = MAX(RN_East1[EastSales])   // MAX(Column Name)<br>
MinSales = MIN(RN_East1[EastSales])   // MIN(Column Name)<br>
SDSales = STDEV.S(RN_East1[EastSales])   // STDEV.S(Column Name)<br>
VarSales = VAR.S(RN_East1[EastSales])   // VAR.S(Column Name)<br>
SDSales1 = SQRT(VAR.S(RN_East1[EastSales]))   // SQRT(VAR.S(Column Name))<br>
VarSales1 = STDEV.S(RN_East1[EastSales])^2   // STDEV.S(Column Name) ^ 2<br>
GSTSalesSumX = SUMX(RN_East1, RN_East1[EastSales] * 0.18)   // SUMX(Table Name, Expression)<br>
GSTSalesAvgX = AVERAGEX(RN_East1, RN_East1[EastSales] * 0.18)   // AVERAGEX(Table Name, Expression)<br>
GSTSalesMinX = MINX(RN_East1, RN_East1[EastSales] * 0.18)   // MINX(Table Name, Expression)<br>
GSTSalesMaxX = MAXX(RN_East1, RN_East1[EastSales] * 0.18)   // MAXX(Table Name, Expression)<br>
CountOfRows = COUNTROWS(RN_East1)   // COUNTROWS(Table Name)<br>
CountXOfRows = COUNTAX(RN_East1, RN_East1[EastSales] * 0.18)   // COUNTAX(Table Name, Expression)<br>
CalculateMinGST = CALCULATE([TotalSales] * 0.18, RN_East1[Month] = "AUG", RN_East1[Product] = "P013")   // CALCULATE(Expression, Filter1, Filter2, ...)<br>
FilterMinGST = MINX(FILTER(RN_East1, RN_East1[Month] = "AUG"), [TotalSales] * 0.18)   // FILTER(Table Name, Filter)<br>
TotalSalesAll = CALCULATE(sum(RN_East1[EastSales]), ALL(RN_East1))   // ALL(Table Name[<Column>])<br>


