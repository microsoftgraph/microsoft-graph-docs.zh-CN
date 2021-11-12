---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29f20bfb6e3cc9d31b6c176af15e60c9cdc9f705
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60945626"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/387566cc-38ae-4e85-ab4b-cd2dd34faa07/siteSources"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEdiscoverySiteSource *siteSource = [[MSGraphEdiscoverySiteSource alloc] init];
MSGraphSite *site = [[MSGraphSite alloc] init];
[site setWebUrl:@"https://contoso.sharepoint.com/sites/SecretSite"];
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