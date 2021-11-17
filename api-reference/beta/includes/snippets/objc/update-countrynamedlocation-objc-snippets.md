---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ade298ccd3ce5654659da1f6498be5daec7c4046a7e17bc1c6be6ec48852a3c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277636"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959"]]];
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