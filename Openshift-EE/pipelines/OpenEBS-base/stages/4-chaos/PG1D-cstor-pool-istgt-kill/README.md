### Verify applicaton availablity post cstor target istgt container kill.

#### Description
Induce cstor target istgt container kill and check if it doesn't affect the application availability.

#### Prerequisites
- OpenShift Cluster should be created and have the dependencies installed.
- cStor based storage pool should have been created.
- OpenEBS storage class should be created with the desired storage pool claim.

#### Procedure
- Deploy statefulset application consuming OpenEBS Volume.
- Check if the application is deployed successfully.
- Induce cstor target istgt container kill and verify if application is running successfully.
- Deprovision statefulset application.

#### Test Result