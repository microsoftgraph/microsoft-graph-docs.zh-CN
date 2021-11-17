---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00e78ee7a512c29d9bfe8a40a4ff5765fec4f35584aba53aa9c4c9d5fab9301c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220332"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/conditionalAccess/namedLocations"]]];
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