# State-of-the-Art-AI-Forecasting-Software

## About This Project

This repository contains an integrated AI-driven material planning system developed to eliminate supply chain uncertainties and bullwhip effects. The software was created during my 6-month internship (June-December 2025) to address critical forecasting and planning challenges in challenging manufacturing environments.

<img width="1917" height="676" alt="image" src="https://github.com/user-attachments/assets/8ec73891-2fde-409c-9a49-697c60e1d77e" />

<img width="1918" height="574" alt="image" src="https://github.com/user-attachments/assets/2764e61c-2620-41a7-8835-33364a17a818" />


## What This Software Does

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/3e0ec818-70a4-4189-87c0-43e10e818254" />



This AI system transforms material planning by providing:
- **Accurate Forecasting**: Uses State-of-the-Art AI for superior prediction accuracy 
- **Cost Optimization**: Calculates potential savings through improved forecasting
- **Real-time Analytics**: Interactive dashboards with Excel export capabilities
- **Risk Assessment**: Supplier network and lead time variability analysis and fuzzy logic
- **Dynamic Learning**: Future scenario optimization using evolutionary computation

The software processes historical usage, forecast, supplier, and financial data to generate actionable insights for material planners.

## Sample Excel Results

<img width="1097" height="1024" alt="image" src="https://github.com/user-attachments/assets/a9802806-acfd-4d70-bd26-3fdc3035eec6" />

<img width="1175" height="1024" alt="image" src="https://github.com/user-attachments/assets/50e0cf30-debb-4fb7-ae7f-66aa47517d8a" />

<img width="1919" height="971" alt="image" src="https://github.com/user-attachments/assets/9bd64eb4-d1c7-42a7-9e48-305db517fb21" />

<img width="1199" height="1023" alt="image" src="https://github.com/user-attachments/assets/636ec58c-7556-4522-b548-406c5f746495" />


## Key Technologies & Architecture

<br/><img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/2a45f582-0f07-40dd-9ec3-ca43625b44f7" /><br/>

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/b93554a2-2d97-4a25-8641-85dd0f74c387" /><br/>

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/3a4ee1ec-4973-4f00-b238-0de09891327b" /><br/>


### AI Framework
- **TabPFN (Tabular Prior Data Fitted Network)**: Transformer-based neural network for tabular data forecasting
- **Evolutionary Computation**: Multi-objective optimization for scenario planning
- **Ensemble AI Models**: Multiple specialized models working in parallel

### UML Class Diagram (Work in Progress)

<img width="4758" height="4200" alt="Packages" src="https://github.com/user-attachments/assets/2f695523-5623-4869-8dce-5b4c89caa0f1" />


Encapsulation – Each class groups related data and methods together (e.g., Main, DynamicClassifier), controlling access to internal details through attributes and functions.

Abstraction – Complex operations are hidden behind clear interfaces (e.g., FinancialCalculations, DynamicLearningTab) so users interact only with necessary functionality.

Inheritance – Shared structures and behaviors are extended by specialized classes (e.g., DynamicLearningTab inherits from DynamicClassifierBase).

Polymorphism – Different classes implement methods that can be used interchangeably (e.g., various calculation and tab classes override or extend base behaviors for specific contexts).


### System Capacity
- **Maximum Dataset**: 5,000 material codes with 120 months of data
- **Processing Time**: Small datasets easily take less than 5 minutes. Large Datasets do not take more than 1hr 30 mins.
- **Interface Display**: Limited to 100 rows (full data available in Excel export)

### Runtime Estimates
Processing time depends on dataset size and complexity. Even the maximum dataset size will not take longer than 1hr 15mins.

## Getting Started

### Prerequisites
- Windows Operating System
- Python 3.11.0
- Admin privileges for installation
- Access to company ServiceNow portal

### Quick Start
1. **Download Python 3.11.0** from official Python website
   
3. **Install Python** (ensure "Add to Path" is checked)
   
5. **Locate the Python exe and add it as an Environment Variable under Path.** It will be somewhere which looks like
   C:\Users\<USER>\AppData\Local\Programs\Python
  
7. **Clone/Download** this repository
   
9. **CD to the unzipped folder and Install Dependencies**: 
   ```bash
   pip install -r requirements.txt
   ```

10. **Run the Application** using the provided .bat file

### Creating Desktop Shortcuts
- Right-click the .bat file → "Copy as path"
- Desktop → Right-click → "New" → "Shortcut" → Paste path
- Name it "AI Software"

## How to Use

### 1. Prepare Your Data
Create an Excel file with these **exact** sheet names:
- `Historical Forecast` - 60 months of ad hoc order data
- `Historical Usage` - 60 months based on actual transactions
- `Supplier Performance` - 60 months of PO performance data
- `Financial Standard Price` - Latest pricing data
- `Current Inventory` - Current stock levels
- `Financial Extra Cost Data` - Write-off, scrap, and premium freight costs

You may generate a sample dataset and fit in your data based on the provided format

### 2. Run Analysis
1. Launch the software using your created shortcut
2. Upload your prepared Excel file (You may generate a sample dataset)
3. Click "Run all Data Analysis". 
4. Wait for processing (may take over 1hr for very large datasets)
5. Export results to Excel (You may also shortcut to exporting to Excel immediately)

### 3. Interpret Results

**Tab 1 - Exploratory Data Analysis**: Overview of material patterns and supplier completeness

**Tab 2 - Cost Savings & Forecasting**: 
- MAPE accuracy metrics (lower = better)
- Cost variance calculations
- TabPFN vs. Historical forecast comparison

**Tab 3 - Dynamic Optimization**: 
- Future scenario planning
- Risk-adjusted forecasting
- Order adjustment recommendations

**Tab 4 - Final Actions**
- Unique to the Excel Export
- Fast and Straightforward decision guidance

## Troubleshooting

### Common Issues

1. **Python Version Check**:
   ```bash
   py
   ```
   Should display Python 3.11.0 version details

2. **Environment Variables**: Verify Python is added to PATH in Environment Variables

3. **Library Installation**: Run the library version check script provided in the project folder

4. **Loading Bar Issues**:
   - Data generation: May pause at 95% while writing to Excel (normal)
   - Analysis: May show "not responding" at 100% while processing (normal)

### Performance Guidelines
- Maximum dataset: 5,000 material codes with 120 months of data
- Analysis runtime varies by dataset size (refer to runtime estimate tables)
- Interface displays are capped at 100 rows for performance


### System Design
- Modular architecture with clear separation of concerns
- Polymorphic data handling for different input formats
- Secure development practices with proper encapsulation
- Session-based memory management


## Future Roadmap

### Current Scope
Focus on consumption-based forecasting accuracy for material planning.

### Future Enhancements

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/7efdba72-f23e-4947-bcdb-9d1b4a476ce9" />



- Integration with Production Planning (MPS, capacity planning, scheduling)
- Industrial Engineering workflows (process improvement, bottleneck analysis)
- Enhanced Material-Production integration (MPS validation, load balancing)

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/582e1b03-e975-401e-a060-ca7c9b73d250" />



## License

This project was developed as part of an internship program. Please refer to your organization's software and AI usage policies.

## Contact & Support

For technical issues or questions about implementation, documentation has been uploaded for your reference.

