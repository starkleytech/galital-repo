to build the rpms
* 1 - Move the rpmbuild directory to /root/ with rsync -avh rpmbuild /root/
* 2 - build the rpm, first it has to download the nodes, or you manually put the nodes in the SOURCES folder. These SHOULD be included if your downloading this repository, if not, replace as needed and update the file names in the SPECS/appropriate.spec file. aka, its not automated for the build, if its not already there.
* 3 - from the /root/rpmbuild directory run 'rpmbuild -ba SPECS/<spec file you want to build>.spec
This will produce a source rpm in the SRPMS dir, and a production rpm in the RPMS dir

