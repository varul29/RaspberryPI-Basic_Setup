# Create Firebase Setup
 
 Log in to firebase console.
  
  - Click on "Add Project"
  
  ![alt text](https://github.com/varul29/Raspberry-PI-/blob/master/Add%20project.PNG)
  
  - Write Project name. 
  
  - Accept controller-controller terms.
    
  ![alt text](https://github.com/varul29/Raspberry-PI-/blob/master/Project%20name.PNG)
  
  - Click "create project".
  
  - Click "Database" (mentioned in left handside).
  
  ![alt text](https://github.com/varul29/Raspberry-PI-/blob/master/Database.PNG)
  
  - Click on "Create Database".
  
  ![alt text](https://github.com/varul29/Raspberry-PI-/blob/master/Create%20databse.PNG)
  
  - According to newwer version - you can choose either locked version or unlocked version and press Ok.
  
  - Choose Realtime Database(mentioned in the image).
  
  ![alt text](https://github.com/varul29/Raspberry-PI-/blob/master/Real%20time%20database.PNG)
  
  - Click on "Rules".
  
  ![alt text](https://github.com/varul29/Raspberry-PI-/blob/master/Rules.PNG)
  
  ### If in default security rules code is mentioned like below
      
        {
          "rules": { 
            "read": "auth != null"
            "write": "auth != null"
            }
         }
  ### Then change "auth != null" into "true"
  
        {
              "rules": { 
                "read": "true"
               "write": "true"
                }
         }
         
  - click on "Publish".
  
  ![alt text](https://github.com/varul29/Raspberry-PI-/blob/master/ruels%20change.PNG)
  
  - While creating code, we have to use the Host Id "https://tahsensor.firebase.com/" (which will be different for every users)
  
  ![alt text](https://github.com/varul29/Raspberry-PI-/blob/master/hostid.PNG)
  
 At last after performing all the certain parameters mentioned above as well as for different sensor code, 
 The output of database will be appear as mentioned below in snap.
 
  ![alt text](https://github.com/varul29/Raspberry-PI-/blob/master/Sample%20Data.PNG)
 
 
 
      



