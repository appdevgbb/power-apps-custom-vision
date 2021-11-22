# Power Apps Custom Vision Demo 🦝 🐍 🐈 👀

Demo of Power Apps + Custom Vision Object Detection 

<img width="520" alt="Architecture Diagram" src="https://user-images.githubusercontent.com/1610195/142134341-cf0ad2e5-7702-48a3-8615-3698313f3da4.png">

### Prerequisites 📝

* [Custom Vision](customvision.ai) Object Detection Project:
  * [Quickstart](https://docs.microsoft.com/en-us/azure/cognitive-services/custom-vision-service/get-started-build-detector#create-a-new-project)
  * Train your models
  * Publish the most recent iteration of the Prediction API and note the **published-name** on the **Performance** page.
  * Under the **Settings** menu, also note the Project ID.
* Access to Power Apps + premium connectors:
  * [Developer Plan](https://powerapps.microsoft.com/en-us/developerplan)
* Create Azure Blob Storage container for images
  * [Quickstart](https://docs.microsoft.com/en-us/azure/storage/blobs/storage-quickstart-blobs-portal#create-a-container) 
 
### Setup Power App 🔧

* [Import Power Apps solution](https://docs.microsoft.com/en-us/powerapps/maker/data-platform/import-update-export-solutions) in this repository.
* When you import the solution, it will prompt for creation of connections for Azure Blob Storage and Custom Vision. Create the connections and be sure they are selected.
* When you open the application, it will also ask you to allow access to these connections.
* Replace global variables:
  * Open the Custom Vision application in Power Apps. In **App** > **OnStart**, set the published name of the Prediction API, the project ID from Custom Vision, the name of the Azure Blob Storage instance, and the path of folder where the images are contained. 
  * Save the Canvas Application, close and reopen the application to refresh the global variables.
 
<br>

<img width="536" alt="Screen capture from Custom Vision Portal" src="https://user-images.githubusercontent.com/1610195/142933683-f9f5eafe-32b9-4383-8875-842a7a7aa89b.png">
     
<br>

<img width="1429" alt="Screen capture from Power Apps Variables" src="https://user-images.githubusercontent.com/1610195/142933782-243cdd25-480e-472f-9635-f73dbbd0e9e7.png">

### Using the Power App 🤹

* Select an image to upload within the application and press the **Detect Objects** button to show the bounding boxes around the image and the object classifications.

<br>

<img width="1014" alt="Application Demo" src="https://user-images.githubusercontent.com/1610195/141733329-9d02530f-8770-4300-a9c4-128fba3d4c4a.png">

<br>

### Additional Resources 🎁
* [Custom Vision Connector](https://docs.microsoft.com/en-us/connectors/cognitiveservicescustomvision/)
* [Custom Vision Quickstart](https://docs.microsoft.com/en-us/azure/cognitive-services/custom-vision-service/get-started-build-detector#create-a-new-project)
* [Cognitive Services using Custom Connectors](https://powerapps.microsoft.com/ca-es/blog/cognitive-services-with-powerapps-using-custom-connectors) (Older blog, but shows Power Apps components for services)
