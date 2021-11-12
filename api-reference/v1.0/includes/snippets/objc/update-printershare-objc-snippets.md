---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ce459cb33f0fd049312d57d05f9e52b9719b4fd9bb5d9d581b6b664435c962f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902236"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/print/shares/{printerShareId}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPrinterShare *printerShare = [[MSGraphPrinterShare alloc] init];
[printerShare setDisplayName:@"PrinterShare Name"];
[printerShare setAllowAllUsers: false];

NSError *error;
NSData *printerShareData = [printerShare getSerializedDataWithError:&error];
[urlRequest setHTTPBody:printerShareData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```