---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4cecf2807d558adf7069a4c67cd31f872233512
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60927053"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/15d80234-8320-4f10-96d0-d98d53ffdfc9/noncustodialdatasources"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEdiscoveryNoncustodialDataSource *noncustodialDataSource = [[MSGraphEdiscoveryNoncustodialDataSource alloc] init];
[noncustodialDataSource setApplyHoldToSource: false];
MSGraphEdiscoveryDataSource *dataSource = [[MSGraphEdiscoveryDataSource alloc] init];
MSGraphSite *site = [[MSGraphSite alloc] init];
[site setWebUrl:@"https://contoso.sharepoint.com/sites/SecretSite"];
[dataSource setSite:site];
[noncustodialDataSource setDataSource:dataSource];

NSError *error;
NSData *noncustodialDataSourceData = [noncustodialDataSource getSerializedDataWithError:&error];
[urlRequest setHTTPBody:noncustodialDataSourceData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```