---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 626d7657d2a70273a82c3ab1342455f23913b49d4a54fe076e76403149ec0306
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221375"
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