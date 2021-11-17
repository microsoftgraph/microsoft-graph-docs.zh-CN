---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef8d19e1f2291a4d05c9fc345621a5ff4bd01e3cb32dfda11ac054e7b4316501
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162111"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/bookingBusinesses/Fabrikam@M365B489948.onmicrosoft.com"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphBookingBusiness *bookingBusiness = [[MSGraphBookingBusiness alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```