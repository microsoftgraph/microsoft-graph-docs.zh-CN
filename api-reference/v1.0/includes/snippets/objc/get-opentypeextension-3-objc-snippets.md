---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4be9ff07ba0144a78bce10d45e6c792b6d3fcd57
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612623"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===?$expand=extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphMessage *message = [[MSGraphMessage alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```