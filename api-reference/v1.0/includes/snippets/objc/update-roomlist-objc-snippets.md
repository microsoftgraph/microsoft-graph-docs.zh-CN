---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c587c868f14fe62cce764fb6ecadd765442d7b8a858bf8b02fee8e5b6b3fef9a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904106"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/places/Building1RroomList@contoso.onmicrosoft.com"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPlace *place = [[MSGraphPlace alloc] init];
[place setDisplayName:@"Building 1"];
[place setPhone:@"555-555-0100"];
MSGraphPhysicalAddress *address = [[MSGraphPhysicalAddress alloc] init];
[address setStreet:@"4567 Main Street"];
[address setCity:@"Buffalo"];
[address setState:@"NY"];
[address setPostalCode:@"98052"];
[address setCountryOrRegion:@"USA"];
[place setAddress:address];
MSGraphOutlookGeoCoordinates *geoCoordinates = [[MSGraphOutlookGeoCoordinates alloc] init];
[geoCoordinates setAltitude: null];
[geoCoordinates setLatitude: 47.0];
[geoCoordinates setLongitude: -122.0];
[geoCoordinates setAccuracy: null];
[geoCoordinates setAltitudeAccuracy: null];
[place setGeoCoordinates:geoCoordinates];

NSError *error;
NSData *placeData = [place getSerializedDataWithError:&error];
[urlRequest setHTTPBody:placeData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```