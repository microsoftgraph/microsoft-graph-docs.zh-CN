---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9765ca6a0bc86081e5582f4073632a7df9209ee
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936630"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/conditionalAccess/namedLocations"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphNamedLocation *namedLocation = [[MSGraphNamedLocation alloc] init];
[namedLocation setDisplayName:@"Named location with unknown countries and regions"];
NSMutableArray *countriesAndRegionsList = [[NSMutableArray alloc] init];
[countriesAndRegionsList addObject: @"US"];
[countriesAndRegionsList addObject: @"GB"];
[namedLocation setCountriesAndRegions:countriesAndRegionsList];
[namedLocation setIncludeUnknownCountriesAndRegions: true];

NSError *error;
NSData *namedLocationData = [namedLocation getSerializedDataWithError:&error];
[urlRequest setHTTPBody:namedLocationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```