Notes:
-Edit zHabitat.devSettings.config under Configuration SOl Folder and change 'sourceFolder' according to your env /*This is for Unicorn to work*/
-Edit gulp-config.js under Configuration SOl Folder and change 'websiteRoot' and 'sitecoreLibraries' according to your env /*gulp configurations*/
-Edit publishsettings.targets' 'publishUrl' value to your local site's URL /*for Gulp to work*/
-Every project should have a config under App_config/Include/LayerName/projectname.Serialization.config with the proper <include> and <targetDataStore> filled accordingly /*Unicorn*/
-Unicorn publishing is accomplished via siteURL/unicorn.aspx after the site is published
-When you need to publish your project on the Task Runner Explorer and choose 03-PublishAllProjects
-Gulp in general has multiple advantages over bundles as it allows the developer to perform a lot more tasks on the attached scripts and stylesheets such as linting which is a program that supports verifying code quality



Solution History:
2016-11-08 - TamerM
1. Removed Theming extra solution folder from file structure and added new 'code' and 'serialization' folders for theming module (source: http://helix.sitecore.net/principles/file-structure/modules.html)
2. added new 'code' and 'serialization' folders for website module
3. renamed HelixFinancialServices.Theming to HelixFinancialServices.Foundation.Theming
4. renamed module file name from Helix.FinancialServices.Theming to Theming and the same for Website module
5. Added readme files to theming and website modules
2016-11-10 - TamerM
6. renamed solution to HFS instead of HelixFinancialServices because project names have become too long for VS to accept
7. Added HFS.Foundation.Serialization with Unicorn setup
  -Added unicorn .config to Theming and website projects (*.Serialization.config)
  -Added zHabitat.devSettings.config (for dev env settings)
  -Added Gulp files
  -Added packages.json files (with node_modules folder)
  -Added unicorn.js script file