# Create a SIG Google Earth Engine Account
## Sign up

## Upgrade account to alpha (do we still need to do this?)

## Ensure you've been added to SIG's GCP permission groups
* Ask Kyle or Dawn to add you 
* authenticate with a project 

## Setup GEE Python API
### Earth Engine requires you to authenticate your account credentials to access the Earth Engine API and your chosen Cloud Project. We do this with the `gcloud` python utility
### 1. Download the installer for the `glcoud` command-line python [utility](https://cloud.google.com/sdk/docs/install) from Google
### 2. Run the installer
### 3. Select Single User and use the default Destination Folder
### 4. Leave the Selected Components to Install as-is and click Install
### 5. Leave all four boxes checked, and click Finish. This will open a new command-prompt window and auto run gcloud initialization
### 6. It asks whether yo'd like to log in, type y - this will open a new browser window to a Google Authentication page

![kaza_readme_gcloudInstaller_initializing](https://user-images.githubusercontent.com/51868526/184163126-7505745b-f7c3-4745-bb36-3948d1b9ff76.JPG)

### 7. Choose your Google account that is linked to your Earth Engine account, then click Allow on the next page.

![kaza_readme_gcloudInstaller_InitializingSignIn](https://user-images.githubusercontent.com/51868526/184163514-4604ac83-cdad-4dd8-bc67-c37224d6aafc.JPG)

### 8. You will be redirected to a page that says "You are now authenticated with the gcloud CLI!"
### 9. Go back to your shell that had been opened for you by gcloud. It asks you to choose a cloud project and lists all available cloud projects that your google account has access to. Look for `wwf-sig` and then type the number it is listed as to set your project. 

![kaza_readme_gcloudInstaller_chooseCloudProject_chooseWWF-SIG](https://user-images.githubusercontent.com/51868526/184165192-c602f058-b485-419c-b5ea-401c7087fb9f.JPG)

### 10. Back in your separate shell window, first ensure you are in your custom conda env (running `conda activate env-name`), then run:
```
earthengine authenticate
```
### 11. In the browser window that opens, select the Google account that is tied to your EE account, select the wwf-sig cloud project, then click Generate Token at the bottom of the page.
### 12. On the next page, select your Google account again, then click Allow on the next page.
### 13. Copy the authorization token it generates to your clipboard and back in your shell, paste it and hit Enter. 

# Testing Your Setup
### Test that earthengine is setup and authenticated by checking the folder contents within the `wwf-sig` cloud project. 
### * In your shell, run:
```
earthengine ls projects/wwf-sig/assets/kaza-lc
```

![kaza_earthenginels](https://user-images.githubusercontent.com/51868526/184402268-5876a8eb-7e1d-4d1f-aef6-658c6e20fe8c.JPG)

If you do not get an error and it returns a list of folders and assets similar to this then you are good to go! :tada:
