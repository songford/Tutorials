---
title: An Open Data Protocol (OData) primer for developers
description: Learn how to explore the data in an OData service, and the functionality included in the service.
tags: [tutorial:product/hcp, tutorial:product/sapui5_web_ide, tutorial:product/mobile, tutorial:technology/odata]
---

## Prerequisites
 - **Proficiency:** Intermediate
 - **Tutorials:** [Localizing your SAPUI5 app](http://go.sap.com/developer/tutorials/hcp-webide-localizing-app.html)

## Next Steps
 - Inserting OData query options into your SAPUI5 app (coming soon)

## Details

### You will learn
Throughout this tutorial series you’ve been working on an app that consumes an OData service. Since you are now familiar with using the content, its time to learn a bit more about what the OData protocol can do for a developer. In the next tutorial, you will learn how to apply these capabilities to your SAPUI5 app.

### Time to Complete
**10-15 min**

---

    
    > Note: if you would like to access an SAP Gateway server, see the Optional section at the end of this tutorial for the free Gateway trial sign up link and OData service URL.


 


 
    ![orderby ProductName descending](https://raw.githubusercontent.com/SAPDocuments/Tutorials/master/tutorials/hcp-webide-odata-primer/mob3-4_18.png)
 

Here is a short summary of the various URLs and query options covered in this tutorial:
 :-------------------------| :-------------
 Service Document             |  <http://services.odata.org/V2/Northwind/Northwind.svc/> 
 Metadata Document            |  <http://services.odata.org/V2/Northwind/Northwind.svc/$metadata>
 View a Collection            |  <http://services.odata.org/V2/Northwind/Northwind.svc/Products>
 Collection with `$skiptoken` |  <http://services.odata.org/V2/Northwind/Northwind.svc/Products?$skiptoken=20>
 Use `$format` to output JSON  |  <http://services.odata.org/V2/Northwind/Northwind.svc/Products?$format=json>
 `$select` to define a subset of fields to return and `$expand` to include a `NavigationProperty` linked entity in the results |  <http://services.odata.org/V2/Northwind/Northwind.svc/Products?$format=json&$select=ProductName,UnitPrice,Supplier&$expand=Supplier>
If you would like to build an app similar to what you have done in this tutorial series but with "SAP-like" data, you can register for a free [SAP Gateway trial](https://supsignformsb03be6e80.us1.hana.ondemand.com/SUPSignForms/).

The two OData Service document URLs are:
 
 - <https://sapes4.sapdevcenter.com/sap/opu/odata/IWBEP/GWDEMO/>
 - <https://sapes4.sapdevcenter.com/sap/opu/odata/IWFND/RMTSAMPLEFLIGHT/>

To build an app like what you have now, but with data from SAP Gateway you simply need to:

 - Create an HCP destination pointing to `https://sapes4.sapdevcenter.com` following an [earlier tutorial procedure]()
 - Enter the remaining part of the URL in the Data Connection portion of the Web IDE template customization. For the two URLs above, they would be:
  - `/sap/opu/odata/IWBEP/GWDEMO` 
  - `/sap/opu/odata/IWFND/RMTSAMPLEFLIGHT`

 
## Next Steps
 - Inserting OData query options into your SAPUI5 app (coming soon)