# VCheckerNpmCnt


VCheckerNpmCnt is a Docker container which checks if an artifact in a determinate version is located in npmjs.org repositories. 

### VCheckerNpmCnt 
gets the data about the artifacts from a json file with this structure

            {"artifacts":[
				{"artifact":"artifact_1_Name","version":"artifact_1_Version"},
				{"artifact":"artifact_2_Name","version":"artifact_2_version"}
				...
			    ]	
            }

 To get VCheckerNopCnt docker container : docker pull ugenio/vcheckernpmcnt
 To run the container: docker run -v [path to json file]:/usr/src/mymaven/[json name] -e "REPOSITORIES=[json name]" ugenio/vcheckernpmcnt
