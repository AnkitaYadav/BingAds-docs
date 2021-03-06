---
title: UrlSearchParameter Data Object - Ad Insight
ms.service: bing-ads-ad-insight-service
ms.topic: article
author: eric-urban
ms.author: eur
description: The URL search parameter that you can use as a seed for new keyword ideas.
---
# UrlSearchParameter Data Object - Ad Insight
The URL search parameter that you can use as a seed for new keyword ideas.

## Syntax
```xml
<xs:complexType name="UrlSearchParameter" xmlns:xs="http://www.w3.org/2001/XMLSchema">
  <xs:complexContent mixed="false">
    <xs:extension base="tns:SearchParameter">
      <xs:sequence>
        <xs:element minOccurs="0" name="Url" nillable="true" type="xs:string" />
      </xs:sequence>
    </xs:extension>
  </xs:complexContent>
</xs:complexType>
```

## <a name="elements"></a>Elements

|Element|Description|Data Type|
|-----------|---------------|-------------|
|<a name="url"></a>Url|The URL of your website or a page on your website.<br/><br/> Bing Ads extracts keywords from the HTML code on your website or landing page. If your HTML code contains Javascript, which generates content at runtime, Bing Ads will not extract keywords rendered from the Javascript and you'll see fewer or no keywords.|**string**|

## Requirements
Service: [AdInsightService.svc v12](https://adinsight.api.bingads.microsoft.com/Api/Advertiser/AdInsight/v12/AdInsightService.svc)  
Namespace: http\://schemas.datacontract.org/2004/07/Microsoft.BingAds.Advertiser.AdInsight.Api.DataContract.V12.Entity.SearchParameters  

