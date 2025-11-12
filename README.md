# 📊 Monthly Assessment Marks Automation using n8n 🤖

## Description
Automated workflow to calculate monthly assessment marks for DA and DS students using **n8n** 🤖. Collects module-wise scores via forms, computes average marks 📊, and provides eligibility status for the placement drive 🎓.  

The workflow also highlights **weak modules with corresponding marks ⚠️**, helping students focus on areas that need improvement.

## Features
- Collects marks for each module via n8n Form 📝
- Calculates average marks automatically
- Determines eligibility for placement drive
  - ✅ Eligible if average > 70
  - ⚠ Not Eligible if average ≤ 70, with feedback on weak modules
- Displays **weak modules with marks**
- Supports both DA and DS students with respective modules

## Modules
**DA Students:**  
- Python Programming  
- Exploratory Data Analysis (EDA)  
- SQL  
- Power BI  
- Advance Statistics  

**DS Students:**  
- Python Programming  
- Exploratory Data Analysis (EDA)  
- SQL  
- Power BI  
- Advance Statistics  
- Machine Learning (ML)  
- Artificial Neural Networks (ANN)  
- Convolutional Neural Networks (CNN)  
- Natural Language Processing (NLP)  
- Generative AI (GenAI)  

## Workflow Steps
1. **Create Form:** Collect module-wise marks for DA/DS students  
2. **n8n Integration:** Use Form node to get responses  
3. **Calculate Average:** Python or Function node to compute average  
4. **IF Node:** Check eligibility  
   - True: 🎉 “Congratulations! You are eligible for the placement drive.”  
   - False: ⚠ “You are not eligible. Focus on weak modules” + **list of weak modules with marks**  
5. **Output & Test:** Submit responses to validate workflow

## How to Use
1. Open the n8n workflow  
2. Connect the Form node to capture student marks  
3. Use Function node to calculate average and generate weak modules list  
4. Configure IF node to check eligibility  
5. Run the workflow and test with sample submissions  


## License
This project is for educational purposes.
