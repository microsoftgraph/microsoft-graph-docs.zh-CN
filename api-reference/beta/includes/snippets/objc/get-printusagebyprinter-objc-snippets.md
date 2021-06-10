---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c174b857e14afa704b08081822a21d0f11a20542
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869903"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/print/reports/dailyPrintUsageByPrinter/016b5565-3bbf-4067-b9ff-4d68167eb1a6"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphPrintUsageByPrinter *printUsageByPrinter = [[MSGraphPrintUsageByPrinter alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```