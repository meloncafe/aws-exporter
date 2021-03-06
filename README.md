AWS Exporter Usage
=============

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/e4830b435cab41079e36fdc8f1b86143)](https://app.codacy.com/manual/anthunt01/aws-exporter?utm_source=github.com&utm_medium=referral&utm_content=anthunt/aws-exporter&utm_campaign=Badge_Grade_Dashboard)
[![Build Status](https://travis-ci.org/anthunt/aws-exporter.svg?branch=master)](https://travis-ci.org/anthunt/aws-exporter)
![Maven Package](https://github.com/anthunt/aws-exporter/workflows/Maven%20Package/badge.svg)
![Java CI with Maven](https://github.com/anthunt/aws-exporter/workflows/Java%20CI%20with%20Maven/badge.svg)

AWSExporter extracts configuration information about resources you create in AWS into an Excel file.

:wrench: Installation
-------------

Download [aws-exporter-3.0.0-RELEASE-full.jar](https://github.com/anthunt/aws-exporter/releases/download/3.0.0-RELEASE/aws-exporter-3.0.0-RELEASE-full.jar) to your local path and run install
```
$ java -jar aws-exporter-3.0.0-RELEASE-full.jar
```

:file_folder: Program Structure
-------------
<pre><code>
Your path -
          |- aws-exporter-3.0.0-RELEASE-full.jar
          |- startAWSExporter.bat (created at install)
          |- lib (created at install)
          |- conf (created when running startAWSExport.bat)
               |- env.bat
               |- awsExporter.data
          |- exports (created at export)
</code></pre>

:arrow_forward: Running Program
-------------

```
$ startAWSExporter.bat
```

<p align="center">
  <img src="https://github.com/anthunt/aws-exporter/blob/3.x/running.png?raw=true">
</p>

:pencil: Output Excel File
-------------
Output file will be create in exports directory.
#### Output File Naming Format : 
```
[Access Name][Region Name] AWSExport-[Export time].xlsx
```

:heavy_check_mark: Support AWS Services
-------------

+ VPC
+ Subnet
+ Route Table
+ Internet Gateway
+ Egress Only Internet Gateway
+ NAT Gateway
+ Customer Gateway
+ VPN Gateway
+ VPN Connection
+ Security Group
+ EC2 Instance
+ EBS Volume
+ ElasticLoadBalancer (ALB, NLB, CLB)
+ ElastiCache
+ RDS
+ Key Management Service
+ Certificate Manager
+ Simple Storage Service
+ Direct Connect Connection
+ Direct Connect Location
+ Virtual Gateway
+ Virtual Interface
+ LAG
+ Direct Connect Gateway
+ Directory Service
