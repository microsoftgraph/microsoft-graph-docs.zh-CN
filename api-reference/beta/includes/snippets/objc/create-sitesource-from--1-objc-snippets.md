---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f52a6b22d4fb7da954e772cd98250930e429d2d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60934644"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/15d80234-8320-4f10-96d0-d98d53ffdfc9/custodians/8904528fef4d4578b44f71a80188f400/siteSources"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEdiscoverySiteSource *siteSource = [[MSGraphEdiscoverySiteSource alloc] init];
MSGraphSite *site = [[MSGraphSite alloc] init];
[site setWebUrl:@"https://contoso.sharepoint.com/sites/HumanResources"];
[siteSource setSite:site];

NSError *error;
NSData *siteSourceData = [siteSource getSerializedDataWithError:&error];
[urlRequest setHTTPBody:siteSourceData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```