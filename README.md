# TestCafeDocker
Custom testcafe Dockerfile and docker-compose file.  



Setting the execution script that includes git cloning and testcafe execution steps. An environment arg is set in SCRIPT1 which can be parameterized in Jenkins build.  
 >SCRIPT1="cd TestCafeProjects && sudo git clone http://gitdep**:****@gitlab.info****.com/nau****qa/NGJobsearchDesktopTestCafe.git -b multi && cd NGJobsearchDesktopTestCafe && sudo npm run DockComplete:Chrome:headless" docker-compose up

