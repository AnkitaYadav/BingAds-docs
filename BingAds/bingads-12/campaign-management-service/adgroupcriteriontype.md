---
title: AdGroupCriterionType Value Set - Campaign Management
ms.service: bing-ads-campaign-management-service
ms.topic: article
author: eric-urban
ms.author: eur
description: Defines the possible types of ad group criterions.
---
# AdGroupCriterionType Value Set - Campaign Management
Defines the possible types of ad group criterions.

## Syntax
```xml
<xs:simpleType name="AdGroupCriterionType" xmlns:xs="http://www.w3.org/2001/XMLSchema">
  <xs:list>
    <xs:simpleType>
      <xs:restriction base="xs:string">
        <xs:enumeration value="ProductPartition">
          <xs:annotation>
            <xs:appinfo>
              <EnumerationValue xmlns="http://schemas.microsoft.com/2003/10/Serialization/">2</EnumerationValue>
            </xs:appinfo>
          </xs:annotation>
        </xs:enumeration>
        <xs:enumeration value="Webpage">
          <xs:annotation>
            <xs:appinfo>
              <EnumerationValue xmlns="http://schemas.microsoft.com/2003/10/Serialization/">4</EnumerationValue>
            </xs:appinfo>
          </xs:annotation>
        </xs:enumeration>
        <xs:enumeration value="Targets">
          <xs:annotation>
            <xs:appinfo>
              <EnumerationValue xmlns="http://schemas.microsoft.com/2003/10/Serialization/">8</EnumerationValue>
            </xs:appinfo>
          </xs:annotation>
        </xs:enumeration>
        <xs:enumeration value="Age">
          <xs:annotation>
            <xs:appinfo>
              <EnumerationValue xmlns="http://schemas.microsoft.com/2003/10/Serialization/">16</EnumerationValue>
            </xs:appinfo>
          </xs:annotation>
        </xs:enumeration>
        <xs:enumeration value="Gender">
          <xs:annotation>
            <xs:appinfo>
              <EnumerationValue xmlns="http://schemas.microsoft.com/2003/10/Serialization/">32</EnumerationValue>
            </xs:appinfo>
          </xs:annotation>
        </xs:enumeration>
        <xs:enumeration value="DayTime">
          <xs:annotation>
            <xs:appinfo>
              <EnumerationValue xmlns="http://schemas.microsoft.com/2003/10/Serialization/">64</EnumerationValue>
            </xs:appinfo>
          </xs:annotation>
        </xs:enumeration>
        <xs:enumeration value="Device">
          <xs:annotation>
            <xs:appinfo>
              <EnumerationValue xmlns="http://schemas.microsoft.com/2003/10/Serialization/">128</EnumerationValue>
            </xs:appinfo>
          </xs:annotation>
        </xs:enumeration>
        <xs:enumeration value="Location">
          <xs:annotation>
            <xs:appinfo>
              <EnumerationValue xmlns="http://schemas.microsoft.com/2003/10/Serialization/">256</EnumerationValue>
            </xs:appinfo>
          </xs:annotation>
        </xs:enumeration>
        <xs:enumeration value="LocationIntent">
          <xs:annotation>
            <xs:appinfo>
              <EnumerationValue xmlns="http://schemas.microsoft.com/2003/10/Serialization/">512</EnumerationValue>
            </xs:appinfo>
          </xs:annotation>
        </xs:enumeration>
        <xs:enumeration value="Radius">
          <xs:annotation>
            <xs:appinfo>
              <EnumerationValue xmlns="http://schemas.microsoft.com/2003/10/Serialization/">1024</EnumerationValue>
            </xs:appinfo>
          </xs:annotation>
        </xs:enumeration>
        <xs:enumeration value="Audience">
          <xs:annotation>
            <xs:appinfo>
              <EnumerationValue xmlns="http://schemas.microsoft.com/2003/10/Serialization/">2048</EnumerationValue>
            </xs:appinfo>
          </xs:annotation>
        </xs:enumeration>
        <xs:enumeration value="CustomAudience">
          <xs:annotation>
            <xs:appinfo>
              <EnumerationValue xmlns="http://schemas.microsoft.com/2003/10/Serialization/">4096</EnumerationValue>
            </xs:appinfo>
          </xs:annotation>
        </xs:enumeration>
        <xs:enumeration value="InMarketAudience">
          <xs:annotation>
            <xs:appinfo>
              <EnumerationValue xmlns="http://schemas.microsoft.com/2003/10/Serialization/">8192</EnumerationValue>
            </xs:appinfo>
          </xs:annotation>
        </xs:enumeration>
        <xs:enumeration value="RemarketingList">
          <xs:annotation>
            <xs:appinfo>
              <EnumerationValue xmlns="http://schemas.microsoft.com/2003/10/Serialization/">16384</EnumerationValue>
            </xs:appinfo>
          </xs:annotation>
        </xs:enumeration>
        <xs:enumeration value="CompanyName">
          <xs:annotation>
            <xs:appinfo>
              <EnumerationValue xmlns="http://schemas.microsoft.com/2003/10/Serialization/">32768</EnumerationValue>
            </xs:appinfo>
          </xs:annotation>
        </xs:enumeration>
        <xs:enumeration value="JobFunction">
          <xs:annotation>
            <xs:appinfo>
              <EnumerationValue xmlns="http://schemas.microsoft.com/2003/10/Serialization/">65536</EnumerationValue>
            </xs:appinfo>
          </xs:annotation>
        </xs:enumeration>
        <xs:enumeration value="Industry">
          <xs:annotation>
            <xs:appinfo>
              <EnumerationValue xmlns="http://schemas.microsoft.com/2003/10/Serialization/">131072</EnumerationValue>
            </xs:appinfo>
          </xs:annotation>
        </xs:enumeration>
        <xs:enumeration value="ProductAudience">
          <xs:annotation>
            <xs:appinfo>
              <EnumerationValue xmlns="http://schemas.microsoft.com/2003/10/Serialization/">262144</EnumerationValue>
            </xs:appinfo>
          </xs:annotation>
        </xs:enumeration>
      </xs:restriction>
    </xs:simpleType>
  </xs:list>
</xs:simpleType>
```

## <a name="values"></a>Values

|Value|Description|
|-----------|---------------|
|<a name="age"></a>Age|The ad group criterion is an age criterion.<br/><br/>The *Criterion* element of a [BiddableAdGroupCriterion](biddableadgroupcriterion.md) can be an instance of [AgeCriterion](agecriterion.md). The *CriterionBid* element of a [BiddableAdGroupCriterion](biddableadgroupcriterion.md) must be an instance of [BidMultiplier](bidmultiplier.md) when paired with this criterion type.<br/><br/>Age exclusions with [NegativeAdGroupCriterion](negativeadgroupcriterion.md) are only supported with Audience campaigns.|
|<a name="audience"></a>Audience|The ad group criterion is an audience criterion.<br/><br/>The *Criterion* element of either the [BiddableAdGroupCriterion](biddableadgroupcriterion.md) or [NegativeAdGroupCriterion](negativeadgroupcriterion.md) can be an instance of [AudienceCriterion](audiencecriterion.md). In other words you can include some audiences, and exclude other audiences.<br/><br/>The *CriterionBid* element of a [BiddableAdGroupCriterion](biddableadgroupcriterion.md) must be an instance of [BidMultiplier](bidmultiplier.md) when paired with this criterion type.<br/><br/>To add, delete, or update audience criterions i.e., custom audiences, in-market audiences, product audiences, and remarketing lists, you must specify the *Audience* value. To retrieve these audience criterions via [GetAdGroupCriterionsByIds](getadgroupcriterionsbyids.md) you must request the specific type i.e., *CustomAudience*, *InMarketAudience*, *ProductAudience*, and *RemarketingList*.|
|<a name="companyname"></a>CompanyName|The ad group criterion is a company name profile criterion.<br/><br/>The *Criterion* element of either the [BiddableAdGroupCriterion](biddableadgroupcriterion.md) or [NegativeAdGroupCriterion](negativeadgroupcriterion.md) can be an instance of [ProfileCriterion](profilecriterion.md) where the [ProfileType](profilecriterion.md#profiletype) is set to *CompanyName*. In other words you can include some profiles, and exclude other profiles.<br/><br/>The *CriterionBid* element of a [BiddableAdGroupCriterion](biddableadgroupcriterion.md) must be an instance of [BidMultiplier](bidmultiplier.md) when paired with this criterion type.<br/><br/>This criterion type can only be used with Audience campaigns.|
|<a name="customaudience"></a>CustomAudience|The ad group criterion is a custom audience association.<br/><br/>This criterion type value is only used by the [GetAdGroupCriterionsByIds](getadgroupcriterionsbyids.md) operation to request the custom audience associations represented by the [AudienceCriterion](audiencecriterion.md) objects. To manage the custom audience, see [CustomAudience](customaudience.md). |
|<a name="daytime"></a>DayTime|The ad group criterion is a day and time criterion.<br/><br/>The *Criterion* element of a [BiddableAdGroupCriterion](biddableadgroupcriterion.md) can be an instance of [DayTimeCriterion](daytimecriterion.md), but day and time criterion are not supported with [NegativeAdGroupCriterion](negativeadgroupcriterion.md).<br/><br/>The *CriterionBid* element of a [BiddableAdGroupCriterion](biddableadgroupcriterion.md) must be an instance of [BidMultiplier](bidmultiplier.md) when paired with this criterion type.|
|<a name="device"></a>Device|The ad group criterion is a device criterion.<br/><br/>The *Criterion* element of a [BiddableAdGroupCriterion](biddableadgroupcriterion.md) can be an instance of [DeviceCriterion](devicecriterion.md), but device criterion are not supported with [NegativeAdGroupCriterion](negativeadgroupcriterion.md).<br/><br/>The *CriterionBid* element of a [BiddableAdGroupCriterion](biddableadgroupcriterion.md) must be an instance of [BidMultiplier](bidmultiplier.md) when paired with this criterion type.|
|<a name="gender"></a>Gender|The ad group criterion is a gender criterion.<br/><br/>The *Criterion* element of a [BiddableAdGroupCriterion](biddableadgroupcriterion.md) can be an instance of [GenderCriterion](gendercriterion.md). The *CriterionBid* element of a [BiddableAdGroupCriterion](biddableadgroupcriterion.md) must be an instance of [BidMultiplier](bidmultiplier.md) when paired with this criterion type.<br/><br/>Gender exclusions with [NegativeAdGroupCriterion](negativeadgroupcriterion.md) are only supported with Audience campaigns.|
|<a name="industry"></a>Industry|The ad group criterion is an industry profile criterion.<br/><br/>The *Criterion* element of either the [BiddableAdGroupCriterion](biddableadgroupcriterion.md) or [NegativeAdGroupCriterion](negativeadgroupcriterion.md) can be an instance of [ProfileCriterion](profilecriterion.md) where the [ProfileType](profilecriterion.md#profiletype) is set to *Industry*. In other words you can include some profiles, and exclude other profiles.<br/><br/>The *CriterionBid* element of a [BiddableAdGroupCriterion](biddableadgroupcriterion.md) must be an instance of [BidMultiplier](bidmultiplier.md) when paired with this criterion type.<br/><br/>This criterion type can only be used with Audience campaigns.|
|<a name="inmarketaudience"></a>InMarketAudience|The ad group criterion is an in-market audience association.<br/><br/>This criterion type value is only used by the [GetAdGroupCriterionsByIds](getadgroupcriterionsbyids.md) operation to request the in-market audience associations represented by the [AudienceCriterion](audiencecriterion.md) objects. To manage the in-market audience, see [InMarketAudience](inmarketaudience.md). |
|<a name="jobfunction"></a>JobFunction|The ad group criterion is a job function profile criterion.<br/><br/>The *Criterion* element of either the [BiddableAdGroupCriterion](biddableadgroupcriterion.md) or [NegativeAdGroupCriterion](negativeadgroupcriterion.md) can be an instance of [ProfileCriterion](profilecriterion.md) where the [ProfileType](profilecriterion.md#profiletype) is set to *JobFunction*. In other words you can include some profiles, and exclude other profiles.<br/><br/>The *CriterionBid* element of a [BiddableAdGroupCriterion](biddableadgroupcriterion.md) must be an instance of [BidMultiplier](bidmultiplier.md) when paired with this criterion type.<br/><br/>This criterion type can only be used with Audience campaigns.|
|<a name="location"></a>Location|The ad group criterion is a location criterion.<br/><br/>The *Criterion* element of either the [BiddableAdGroupCriterion](biddableadgroupcriterion.md) or [NegativeAdGroupCriterion](negativeadgroupcriterion.md) can be an instance of [LocationCriterion](locationcriterion.md). In other words you can include some locations, and exclude other locations.<br/><br/>The *CriterionBid* element of a [BiddableAdGroupCriterion](biddableadgroupcriterion.md) must be an instance of [BidMultiplier](bidmultiplier.md) when paired with this criterion type.|
|<a name="locationintent"></a>LocationIntent|The ad group criterion is a location intent criterion.<br/><br/>The *Criterion* element of a [BiddableAdGroupCriterion](biddableadgroupcriterion.md) can be an instance of [LocationIntentCriterion](locationintentcriterion.md), but location intent criterion are not supported with [NegativeAdGroupCriterion](negativeadgroupcriterion.md).<br/><br/>The *CriterionBid* element of a [BiddableAdGroupCriterion](biddableadgroupcriterion.md) must be nil or empty when paired with this criterion type.|
|<a name="productaudience"></a>ProductAudience|The ad group criterion is product audience association.<br/><br/>This criterion type value is only used by the [GetAdGroupCriterionsByIds](getadgroupcriterionsbyids.md) operation to request the product audience associations represented by the [AudienceCriterion](audiencecriterion.md) objects. To manage the product audience, see [ProductAudience](productaudience.md).<br/><br/>This audience type can only be used with Audience campaigns that have a [ShoppingSetting](shoppingsetting.md)).|
|<a name="productpartition"></a>ProductPartition|The ad group criterion is a product partition criterion.<br/><br/>The *Criterion* element of either the [BiddableAdGroupCriterion](biddableadgroupcriterion.md) or [NegativeAdGroupCriterion](negativeadgroupcriterion.md) can be an instance of [ProductPartition](productpartition.md). In other words you can include some product partitions, and exclude other product partitions.<br/><br/>This criterion type is only used with Bing Shopping campaigns.<br/><br/>The *CriterionBid* element of a [BiddableAdGroupCriterion](biddableadgroupcriterion.md) must be an instance of [FixedBid](fixedbid.md) when paired with this criterion type.|
|<a name="radius"></a>Radius|The ad group criterion is a radius criterion.<br/><br/>The *Criterion* element of a [BiddableAdGroupCriterion](biddableadgroupcriterion.md) can be an instance of [RadiusCriterion](radiuscriterion.md), but radius criterion are not supported with [NegativeAdGroupCriterion](negativeadgroupcriterion.md).<br/><br/>The *CriterionBid* element of a [BiddableAdGroupCriterion](biddableadgroupcriterion.md) must be an instance of [BidMultiplier](bidmultiplier.md) when paired with this criterion type.|
|<a name="remarketinglist"></a>RemarketingList|The ad group criterion is a remarketing list association.<br/><br/>This criterion type value is only used by the [GetAdGroupCriterionsByIds](getadgroupcriterionsbyids.md) operation to request the remarketing list associations represented by the [AudienceCriterion](audiencecriterion.md) objects. To manage the remarketing list, see [RemarketingList](remarketinglist.md).|
|<a name="targets"></a>Targets|Represents one or more [AgeCriterion](agecriterion.md), [DayTimeCriterion](daytimecriterion.md), [DeviceCriterion](devicecriterion.md), [GenderCriterion](gendercriterion.md), [LocationCriterion](locationcriterion.md), [LocationIntentCriterion](locationintentcriterion.md), [ProfileCriterion](profilecriterion.md), and [RadiusCriterion](radiuscriterion.md) objects that can be managed together to show ads based on your target criteria.<br/><br/>To add, delete, or update target criterions i.e., age, company name, day and time, device, gender, industry, job function, location, location intent, and radius criterions, you must specify the *CriterionType* value as *Targets*. You can add, delete, and update multiple target criterion types in the same operation. To retrieve these target criterions via [GetAdGroupCriterionsByIds](getadgroupcriterionsbyids.md) you must request the specific type individually i.e., *Age*, *CompanyName*, *DayTime*, *Device*, *Gender*, *Industry*, *JobFunction*, *Location*, *LocationIntent*, and *Radius*.|
|<a name="webpage"></a>Webpage|The ad group criterion is a webpage criterion.<br/><br/>The *Criterion* element of either the [BiddableAdGroupCriterion](biddableadgroupcriterion.md) or [NegativeAdGroupCriterion](negativeadgroupcriterion.md) can be an instance of [Webpage](webpage.md), but webpage criterion are not supported with [BiddableAdGroupCriterion](biddableadgroupcriterion.md). In other words you can include some webpages, and exclude other webpages.<br/><br/>This criterion type can only be used with Dynamic Search Ads campaigns.<br/><br/>The *CriterionBid* element of a [BiddableAdGroupCriterion](biddableadgroupcriterion.md) must be an instance of [FixedBid](fixedbid.md) when paired with this criterion type.|

## Requirements
Service: [CampaignManagementService.svc v12](https://campaign.api.bingads.microsoft.com/Api/Advertiser/CampaignManagement/v12/CampaignManagementService.svc)  
Namespace: https\://bingads.microsoft.com/CampaignManagement/v12  

## Used By
[AddAdGroupCriterions](addadgroupcriterions.md)  
[DeleteAdGroupCriterions](deleteadgroupcriterions.md)  
[GetAdGroupCriterionsByIds](getadgroupcriterionsbyids.md)  
[UpdateAdGroupCriterions](updateadgroupcriterions.md)  
