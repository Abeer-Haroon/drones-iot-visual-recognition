# drones-iot-visual-recognition
This tutorial shows how you can use drone aerial images, Watson Studio, and Watson Visual Recognition to survey wildfire-damaged neighborhoods and identify burned and intact homes.

## Call for Code
Call for Code unites developers and data scientists around the world to create sustainable, scalable, and life-saving open source technologies via the power of Cloud, AI, blockchain and IoT technologies. Check out the link to learn more: https://developer.ibm.com/code-and-response/

## Learning objectives
After completing this tutorial, you will be able to:
1. Create a Visual Recognition model in Watson Studio running in IBM Cloud
2. Capture images from a drone and zip them into a class
3. Train a model to identify objects in the images
4. Score and count the identified objects

## Prerequisites

1. Sign up for an [IBM Cloud account](https://cloud.ibm.com/registration/).
3. Datasets for the visual recognition model. Use these Sample [Datasets](https://github.com/Abeer-Haroon/AI-Treasure-Hunt-With-Watson/blob/master/datasets) or any dataset of your choice.

## Estimated time

This tutorial takes about 20 minutes to complete if you already have an IBM cloud account set up.

 ## Steps
 
First you set up the services on IBM Cloud. Then you set up the client application.

1. Create an instance of the [Watson Visual Recognition](https://www.ibm.com/watson/services/visual-recognition/) service and get your credentials:
   - Go to the [Watson Visual Recognition](https://cloud.ibm.com/catalog/services/visual-recognition) page in the IBM Cloud Catalog.
   - Log in to your IBM Cloud account.
   - Click **Create**.
   - Click **Service Credentials** > New Credentials > Add

![](https://github.com/Abeer-Haroon/AI-Treasure-Hunt-With-Watson/blob/master/images/ath3.png)
   
2. Create an instance of the Watson Studio
   - Go to the [Watson Studio](https://cloud.ibm.com/catalog/services/watson-studio?bss_account=e366b6e4fb004c5eaccfbe7042b670a4) page in the IBM Cloud Catalog.
   - Click **Create**.

![](https://github.com/Abeer-Haroon/AI-Treasure-Hunt-With-Watson/blob/master/images/ath12.png)

   - Click **Get Started**.
 
 ![](https://github.com/Abeer-Haroon/AI-Treasure-Hunt-With-Watson/blob/master/images/ath13.png)
 
    
   - Click **Create a Project** > Visual Recognition
 
 ![](https://github.com/Abeer-Haroon/AI-Treasure-Hunt-With-Watson/blob/master/images/ath14.png)
 

   - Name the project. Select **Storage** > cloud object storage. **Create**
   
3. Creating Visual Recognition Models 

   - Click **Create a Class**. Give it a name. Create at least 2 classes. In this tutorial, 3 classes: "Burned Homes", "Aerial Homes", and "Not Homes".
   - Upload the zip files for the dataset. **Upload to Project** > Browse > Choose folder.
   - Open the class you want to add the dataset to. Click on the uploaded zip folder on the right > **Add to Model**

 ![](https://github.com/Abeer-Haroon/AI-Treasure-Hunt-With-Watson/blob/master/images/ath19.png) 
 
   - Once this is added, Click **Train Model**. This will take some time.
   
![](https://github.com/Abeer-Haroon/AI-Treasure-Hunt-With-Watson/blob/master/images/ath22.png)   
    
 To change the name of the model, edit the following field:
 
 ![](https://github.com/Abeer-Haroon/AI-Treasure-Hunt-With-Watson/blob/master/images/ath23.png) 
 
 
3. Test the Model

   - Upload one of the test images to test your model.

Follow the step-to-step tutorial: https://developer.ibm.com/tutorials/detect-wildfire-damaged-homes-using-drone-images-watson-visual-recognition/
