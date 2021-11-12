---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 776ef34700b8d17b97574d73eee1f64adeec38d5502dc91bb2d38a2406912570
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903102"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/print/printers/86b6d420-7e6b-4797-a05c-af4e56cd81bd/jobs/31216?$expand=documents"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphPrintJob *printJob = [[MSGraphPrintJob alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```