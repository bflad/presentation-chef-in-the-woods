
!SLIDE commandline incremental

    $ cd /path/to/org-app-server-cookbook
    $ vagrant up
    Chef run completed: 100 seconds

!SLIDE commandline incremental smaller

    $ cd /path/to/cheforg
    $ librarian-chef update org-app-server
    Installing org-app-server (1.0.1)
    $ knife spork upload org-app-server
    Freezing org-app-server at 1.0.1...
    Successfully uploaded org-app-server@1.0.1!
    $ knife spork promote development org-app-server --remote
    Adding version constraint org-app-server = 1.0.1
    Saving changes to development.json
    Uploading development.json to Chef Server
    Promotion complete at 2013-04-03 16:05:00 -0400!
