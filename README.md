# Var-Update                                               
                                                                                                                                                            
  Public version registry for Var FiveM resources.                                                                                                          
                                                                                                                                                            
  This repository hosts `versions.json`, which is used by all Var resources to check for available updates at server startup.                               
                                                                                                                                                            
  ## How it works

  Each Var resource includes a `version_check.lua` script that fetches `versions.json` from this repository on startup, compares it with the local version
  defined in `fxmanifest.lua`, and displays a notification in the server console if an update is available.

  ## Automatic updates

  This file is automatically updated via GitHub Actions whenever a new version is pushed to the main repository. Do not edit `versions.json` manually.