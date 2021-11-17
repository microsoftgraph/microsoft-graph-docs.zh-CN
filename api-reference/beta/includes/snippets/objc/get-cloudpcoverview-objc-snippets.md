---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72c788be8bd33ad078c82d98d8d3e9077a32b3667d7f0aa4dfcb6115868d7094
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329032"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/tenantRelationships/managedTenants/cloudPcsOverview/{cloudPcOverviewId}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphCloudPcOverview *cloudPcOverview = [[MSGraphCloudPcOverview alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```