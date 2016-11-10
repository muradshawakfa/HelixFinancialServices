Notes:
-Edit zHabitat.devSettings.config under Configuration SOl Folder and change 'sourceFolder' according to your env
-Edit gulp-config.js under Configuration SOl Folder and change 'websiteRoot' and 'sitecoreLibraries' according to your env
-Every project should have a config under App_config/Include/LayerName/projectname.Serialization.config with the proper <include> and <targetDataStore> filled accordingly
-When you need to publish your project on the Task Runner Explorer and choose 03-PublishAllProjects



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