---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3d32c78483519e15748aa856722c381d8c4f37b5481277514c611a7687f675b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332510"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/educationalActivities/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEducationalActivity *educationalActivity = [[MSGraphEducationalActivity alloc] init];
MSGraphInstitutionData *institution = [[MSGraphInstitutionData alloc] init];
MSGraphPhysicalAddress *location = [[MSGraphPhysicalAddress alloc] init];
[location setType: [MSGraphPhysicalAddressType business]];
[location setPostOfficeBox: null];
[location setStreet:@"12000 E Prospect Rd"];
[location setCity:@"Fort Collins"];
[location setState:@"Colorado"];
[location setCountryOrRegion:@"USA"];
[location setPostalCode:@"80525"];
[institution setLocation:location];
[educationalActivity setInstitution:institution];

NSError *error;
NSData *educationalActivityData = [educationalActivity getSerializedDataWithError:&error];
[urlRequest setHTTPBody:educationalActivityData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```