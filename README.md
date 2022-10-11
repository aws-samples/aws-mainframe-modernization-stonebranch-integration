# aws-mainframe-modernization-stonebranch-integration

This module provides an integration between AWS mainframe modernization service and Stonebranch universal controller to schedule and run batch jobs, embrace automation for mainframe batch running in AWS mainframe modernization service.

The repo has integration template that has to be loaded as a zip to stonebranch product. This will provide option to scheduler and maintain batch jobs.

AWS Services that are used in this solutions are:

- [AWS Mainframe Modernization Service](https://aws.amazon.com/mainframe-modernization/)

## Components details

[assets/template.json](assets/template.json) - This is an universal template that has to be loaded to stonebranch. This template offers configuration of access , batch operations and schedules.

[src/extension/extension.py](src/extension/extension.py) - This python script will resolve the inputs given/configured in the universal template along with the configured credentials and captures the input back to the Stonebranch console.

[src/extension/extension.yml](src/extension/extension.yml) - This file contains the versions and details of the python script.  

[setup.py](setup.py) - A script for bundling and packaging the zip file. The users can download the packaged zip file and upload it into stonebranch console.

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the [LICENSE](LICENSE) file.
