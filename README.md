# DeltaV Edge Environment

The DeltaV Edge Environment provides an easy and secure access to DeltaV system data
for use on premise or in the cloud for monitoring, analytics, reporting or for other
Enterprise applications used to drive operational improvements.

This repository contains example code and resources to facilitate development and deployment of applications written for the edge.

## Getting Started

First, please ensure your Edge Environment has been properly configured and is accessible by your development machine over the network. [You can find further instructions on this step here.]()

### Authentication
Before accessing the Edge REST API data, you need to generate an access token and use
the token for authorization. You may use applications such as Postman or cURL to
generate the token and use it for authentication. [See here for generating access token.]()

### REST API
Once you have received authorization to access the Edge REST API, you can obtain
information (properties and relationships) about the different entities using:
* Query by Path
* Query by Entity ID

| General Form | Query by Path |
|---|---|
| Hierarchy | https://{edge_ip}/edge/api/{version}/graph?path={system_name}/{shortest_unique_path} | 
| Runtime | https://{edge_ip}/edge/api/{version}/graph?path={system_name}/{shortest_unique_path}&p={fields},timestamp | 
| History | https://{edge_ip}/edge/api/{version}/history?path={system_name}/{shortest_unique_path}&p={field} | 

You can find more information on the REST API [here.]()

Below are some examples of sample queries provided in different languages:
<table width=100%>
  <tbody>
    <tr>
      <td>
        <img align="left" width=52px src="https://upload.wikimedia.org/wikipedia/commons/6/6a/JavaScript-logo.png">
        <div>
          <a href="">Writing requests for Edge in JavaScript</a> &nbsp<br/>
        </div>
      </td>
      <td>
        <img align="left" width=52px src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg">
        <div>
          <a href="">Writing requests for Edge in Python (Jupyter Notebook)</a>
        </div>
      </td>
    </tr>
  </tbody>
</table>

## Developing for Edge
### Sample Applications
The fastest way to start writing applications for Edge is with our Jupyter notebook and React web app samples. These resources cover many common use cases of the DeltaV Edge Environment in simple, extensible plug-and-play solutions.

[Getting Started with Jupyter Notebook]()
[Getting Started with React]()
Once you've finished the getting started notebooks, you can then download the linked sample apps and run them locally.

1. [DeltaV Hierarchy Explorer (React app)]()
2. [Real-Time Alert Monitoring Tool (React app)]()
3. [Historical Data Viewer (Jupyter Notebook)]()

### Deploying to Edge Orchestration Marketplace
When you are ready to deploy your application to the Orchestration Marketplace, [follow the instructions here.]() 

Please take a look at our [best practice guidelines]() before upload to ensure adherence. 

## Contributions
If you have a suggestion on how to improve this page or one of our examples, please contact giorgio.guttilla@emerson.com or one of the other project maintainers.
