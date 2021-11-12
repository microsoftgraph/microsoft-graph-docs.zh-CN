---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1457caf4965df54cf666eb0ccb200bf6a7ade865
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60927052"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEdiscoveryNoncustodialDataSource *noncustodialDataSource = [[MSGraphEdiscoveryNoncustodialDataSource alloc] init];
[noncustodialDataSource setApplyHoldToSource: true];
MSGraphEdiscoveryDataSource *dataSource = [[MSGraphEdiscoveryDataSource alloc] init];
[dataSource setEmail:@"adelev@contoso.com"];
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