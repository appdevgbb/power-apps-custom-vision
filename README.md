# Power Apps Custom Vision Demo 🦝 🐍 🐈 👀

Demo of Power Apps + Custom Vision Object Detection 

<img width="520" alt="Architecture Diagram" src="https://user-images.githubusercontent.com/1610195/142134341-cf0ad2e5-7702-48a3-8615-3698313f3da4.png">

### Prerequisites 📝

* [Custom Vision](customvision.ai) Object Detection Project:
  * [Quickstart](https://docs.microsoft.com/en-us/azure/cognitive-services/custom-vision-service/get-started-build-detector#create-a-new-project)
  * Train your models and publish your Prediction API (note the published name).
  * Under the **Settings** menu, also note the Project ID.
* Access to Power Apps + premium connectors:
  * [Developer Plan](https://powerapps.microsoft.com/en-us/developerplan)
 
### Setup Power App 🔧

* [Import Power Apps solution](https://docs.microsoft.com/en-us/powerapps/maker/data-platform/import-update-export-solutions) in this repository.
* Replace global variables
  * In **App** > **OnStart**, set the published name of the Prediction API and the project ID from Custom Vision:  
  * Save the Canvas Application, close and reopen the application to refresh the global variables.
  
<img width="1413" alt="Screen capture from Power Apps" src="https://user-images.githubusercontent.com/1610195/141732628-90e33a6d-a245-4023-baf6-d320ae990571.png">

### Using the Power App 🤹

* Select an image to upload within the application and press the **Detect Objects** button to show the bounding boxes around the image and the object classifications.

<br>

<img width="1014" alt="Application Demo" src="https://user-images.githubusercontent.com/1610195/141733329-9d02530f-8770-4300-a9c4-128fba3d4c4a.png">

<br>

### Additional Resources 🎁
* [Custom Vision Connector](https://docs.microsoft.com/en-us/connectors/cognitiveservicescustomvision/)
* [Custom Vision Quickstart](https://docs.microsoft.com/en-us/azure/cognitive-services/custom-vision-service/get-started-build-detector#create-a-new-project)
* [Cognitive Services using Custom Connectors](https://powerapps.microsoft.com/ca-es/blog/cognitive-services-with-powerapps-using-custom-connectors) (Older blog, but shows Power Apps components for services)
