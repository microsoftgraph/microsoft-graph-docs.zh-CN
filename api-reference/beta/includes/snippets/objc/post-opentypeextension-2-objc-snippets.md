---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b820bc69e4a6630207b06a5a637e6c5b15d35e49
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729278"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphExtension *extension = [[MSGraphExtension alloc] init];
[extension setExtensionName:@"Com.Contoso.Referral"];
[extension setCompanyName:@"Wingtip Toys"];
[extension setDealValue: 500050];
[extension setExpirationDate: "2015-12-03T10:00:00Z"];

NSError *error;
NSData *extensionData = [extension getSerializedDataWithError:&error];
[urlRequest setHTTPBody:extensionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```