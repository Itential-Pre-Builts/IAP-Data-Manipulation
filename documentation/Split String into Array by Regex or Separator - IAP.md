# Split String into Array by Regex or Separator - IAP

## Table of Contents

- [Split String into Array by Regex or Separator - IAP](#split-string-into-array-by-regex-or-separator---iap)
  - [Table of Contents](#table-of-contents)
  - [Overview](#overview)
  - [Getting Started](#getting-started)
    - [Supported IAP Versions](#supported-iap-versions)
    - [External Dependencies](#external-dependencies)
    - [Adapters](#adapters)
    - [How to Install](#how-to-install)
    - [Testing](#testing)
  - [Using this Transformation Project](#using-this-transformation-project)
    - [Entry Point IAP Component](#entry-point-iap-component)
    - [Inputs](#inputs)
    - [Outputs](#outputs)
    - [Query Output](#query-output)
    - [Example Inputs and Outputs](#example-inputs-and-outputs)
    - [API Links](#api-links)
  - [Support](#support)

## Overview

Split a string into an array by regex or another string

Capabilities include:
- This transformation allows IAP users to split a string into an array by regex or another string





## Getting Started

### Supported IAP Versions

Itential Transformation Projects are built and tested on particular versions of IAP. In addition, Transformation Projects are often dependent on external systems and as such, these Transformation Projects will have dependencies on these other systems. This version of **Split String into Array by Regex or Separator - IAP** has been tested with:


- IAP **2023.2**



### External Dependencies

No external dependencies required to run this Transformation Project.




### Adapters

No adapters required to run **Split String into Array by Regex or Separator - IAP**.


### How to Install

To install the Transformation Project:

- Verify you are running a supported version of the Itential Automation Platform (IAP) as listed above in the [Supported IAP Versions](#supported-iap-versions) section in order to install the Transformation Project.
- Import the Transformation Project in [Admin Essentials](https://docs.itential.com/docs/importing-a-prebuilt-4).

### Testing

While Itential tests this Transformation Project and its capabilities, it is often the case the customer environments offer their own unique circumstances. Therefore, it is our recommendation that you deploy this Transformation Project into a development/testing environment in which you can test the Transformation Project.

## Using this Transformation Project


### Entry Point IAP Component

The primary IAP component to run **Split String into Array by Regex or Separator - IAP** is listed below:

<table>
  <thead>
    <tr>
      <th>IAP Component Name</th>
      <th>IAP Component Type</th>
    </tr>
  </thead>
  <tbody>
      <td>Split String into Array by Regex or Separator - IAP</td>
      <td>Transformation</td>
    </tr>
  </tbody>
</table>

### Inputs

The following table lists the inputs for **Split String into Array by Regex or Separator - IAP**:

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Required</th>
      <th>Description</th>
      <th>Example Value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>inputString</td>
      <td>string</td>
      <td>yes</td>
      <td>String to be splitted into array</td>
      <td><pre lang="json">Hello123world-456,2024</pre></td>
    </tr>    <tr>
      <td>separatorString</td>
      <td>string</td>
      <td>yes</td>
      <td>String used as a separator. If "separatorString" and "separatorRegex" are included, "separatorString" is used by default and the "separatorRegex" is ignored</td>
      <td><pre lang="json">o</pre></td>
    </tr>    <tr>
      <td>separatorRegex</td>
      <td>string</td>
      <td>yes</td>
      <td>Regex pattern used as a separator. If "separatorString" and "separatorRegex" are included, "separatorString" is used by default and the "separatorRegex" is ignored</td>
      <td><pre lang="json">/\d+/gm</pre></td>
    </tr>    <tr>
      <td>limit</td>
      <td>['integer', 'null']</td>
      <td>no</td>
      <td>A non-negative integer specifying a limit on the number of substrings to be included in the array</td>
      <td><pre lang="json">2</pre></td>
    </tr>
  </tbody>
</table>



### Outputs

The following table lists the outputs for **Split String into Array by Regex or Separator - IAP**:

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
      <th>Example Value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>splitArray</td>
      <td>array</td>
      <td>Array of substrings</td>
      <td><pre lang="json">[
  "Hello",
  "world-",
  ",",
  ""
]</pre></td>
    </tr>
  </tbody>
</table>



### Query Output

There are no query output examples for **Split String into Array by Regex or Separator - IAP**.




### Example Inputs and Outputs

  
#### Example 1

    
Input:
<pre>{
  "inputString": "Hello123world-456,2024",
  "separatorString": "",
  "separatorRegex": "/\d+/gm",
  "limit": null
} </pre>

    
    
Output:
<pre>[
  "Hello",
  "world-",
  ",",
  ""
] </pre>

    
  
#### Example 2

    
Input:
<pre>{
  "inputString": "Hello123world-456,2024",
  "separatorString": "o",
  "separatorRegex": "/\d+/gm",
  "limit": 2
} </pre>

    
    
Output:
<pre>[
  "Hell",
  "123w"
] </pre>

    
  


### API Links
As noted on the JSON Schema Transformation (JST) Designer documentation for [Using a Method](https://docs.itential.com/docs/jst-designer-2023-1#using-a-method), select the information `(i)` icon in the header of the method to be redirected to the [Mozilla Developer Network JavaScript reference documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference) for the method. 

<table>
  <thead>
    <tr>
      <th>API Name</th>
      <th>API Documentation Link</th>
      <th>API Link Visibility</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>IAP JSON Schema Transformation (JST) Designer</td>
      <td><a href="https://docs.itential.com/docs/jst-designer-2023-1">https://docs.itential.com/docs/jst-designer-2023-1</a></td>
      <td>Public</td>
    </tr>    <tr>
      <td>Using Transformations in IAP Workflows</td>
      <td><a href="https://docs.itential.com/docs/transformation-options-4">https://docs.itential.com/docs/transformation-options-4</a></td>
      <td>Public</td>
    </tr>
  </tbody>
</table>


## Support

Please use your Itential Customer Success account if you need support when using **Split String into Array by Regex or Separator - IAP**.