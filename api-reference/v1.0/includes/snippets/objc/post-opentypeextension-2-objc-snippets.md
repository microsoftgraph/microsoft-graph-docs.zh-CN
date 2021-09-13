---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e480670e99b5f90c66bc38f883e719d49338a11343c31623e0e76a4622c35059
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220007"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions"]]];
[urlRequest setHTTPMethod:@"POST"];

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