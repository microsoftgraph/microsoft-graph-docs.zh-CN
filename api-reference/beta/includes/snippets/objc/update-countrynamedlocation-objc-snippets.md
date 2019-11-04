---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e97e9f809878c6ed8268bd45cdce6542fe85bc9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937105"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphNamedLocation *namedLocation = [[MSGraphNamedLocation alloc] init];
[namedLocation setDisplayName:@"Updated named location without unknown countries and regions"];
NSMutableArray *countriesAndRegionsList = [[NSMutableArray alloc] init];
[countriesAndRegionsList addObject: @"CA"];
[countriesAndRegionsList addObject: @"IN"];
[namedLocation setCountriesAndRegions:countriesAndRegionsList];
[namedLocation setIncludeUnknownCountriesAndRegions: false];

NSError *error;
NSData *namedLocationData = [namedLocation getSerializedDataWithError:&error];
[urlRequest setHTTPBody:namedLocationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```