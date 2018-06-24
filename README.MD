# AWS ElasticSearch Lambda

The lambda function is based on Amazon's native lambda function.  The problem with the original function is that it's not compatible with ElasticCloud or standard ElasticSearch deployment.

## Getting Started

### Installing

Create an S3 bucket and drop zipped up index.js file.  It must be located in the same region where you're planning to deploy the lambda function.

Run the Cloudformation template.  It will prompt you for everything you need for a successful deployment.  This includes:

- bucket name containing the zipped index.js file
- file name ofthe zipped index.js
- name to call the lambda function
- endpoint of Elastic Search
- port number of Elastic Search
- username for Elastic Search
- password for ElasticSearch
- index name (which will have date appended at the end)
