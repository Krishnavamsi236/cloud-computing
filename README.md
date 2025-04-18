# cloud-computing
# Visualizing Data Using Amazon QuickSight

This mini project demonstrates how to visualize data using **Amazon QuickSight**, a cloud-based Business Intelligence (BI) service by AWS. The project involves data collection, uploading to an S3 bucket, and creating interactive dashboards through QuickSight.

---

## 📌 Project Details

## 📖 Abstract

Amazon QuickSight is used to visualize data quickly and effectively. Starting from data preparation to building interactive dashboards, this project showcases:
- Uploading data to Amazon S3
- Connecting QuickSight to the S3 dataset
- Creating graphs like bar charts, line graphs, and pie charts
- Enabling collaboration through shared dashboards
- Automating data refreshes for real-time updates

---

## 🔧 Tools & Technologies Used

- **Amazon S3** - Cloud storage service used to host the dataset
- **Amazon QuickSight** - Used to create dashboards and analyze data
- **Bright Data** - For acquiring large dataset (Amazon Bestseller Dataset)

---

## 🗂️ Resources Used

- `Amazon-Bestseller-Dataset.csv` (Uploaded to S3 bucket)
- JSON configuration for S3 dataset connection
- AWS Console

---

![image](https://github.com/user-attachments/assets/dbf5b508-1845-46c9-b69e-bf598b2b37ba)


## 📈 Procedure

1. **Create an S3 Bucket**
   - Example: `vamsi-project`
   - Upload `Amazon-Bestseller-Dataset.csv` to it

2. **Access BrightData**
   - Download large datasets from [Bright Data](https://brightdata.com)

3. **Prepare JSON Metadata**
   - JSON snippet to define dataset location and format:
     ```json
     {
       "fileLocations": [
         {
           "URIs": ["s3://vamsi-project/Amazon-Bestseller-Dataset.csv"]
         }
       ],
       "globalUploadSettings": {
         "format": "CSV",
         "delimiter": ",",
         "textqualifier": "\"",
         "containsHeader": "true"
       }
     }
     ```

4. **Set Up QuickSight**
   - Sign up via AWS Console
   - Connect QuickSight to the S3 bucket (enable auto-discovery)

5. **Create Dataset in QuickSight**
   - Use the JSON to connect to the S3 data
   - Name and save the dataset

6. **Visualize Data**
   - Drag and drop fields to create:
     - Bar charts
     - Pie charts
     - Line graphs
     - Sorted lists by brand, price, etc.

---

## 📊 Sample Outputs

### Output 1: Alphabetical Bar Graph
Displays products in alphabetical order using bar charts.
![image](https://github.com/user-attachments/assets/543a9434-e029-44b0-b828-c3ccfc6f4f3d)


### Output 2: Top 20 Brands by Price (USD)
A color-coded visualization comparing brand prices.\![image](https://github.com/user-attachments/assets/d38e7e5c-90ba-4749-b992-f3908b59febc)


---

## ✅ Conclusion

Amazon QuickSight provides a user-friendly, powerful platform to:
- Transform raw data into actionable insights
- Build real-time dashboards
- Share reports across teams
- Perform scalable and cost-effective data analysis

This project highlights the ease of integrating S3 with QuickSight and using visualization techniques to uncover hidden patterns.

---

## 📚 References

- [AWS Website](https://aws.amazon.com)
- [Host Static Website on AWS](https://aws.amazon.com/getting-started/projects/host-static-website/faq)
- [Wikipedia - AWS](https://en.wikipedia.org/wiki/Amazon_Web_Services)
- [AWS Free Web Apps](https://aws.amazon.com/free/webapps)
- [Contino: Who’s Using AWS](https://www.contino.io/insights/whos-using-aws)

---

## 💡 Future Scope

- Incorporate live data sources (e.g., from APIs)
- Use ML-powered insights via QuickSight Q
- Embed dashboards in web applications
