---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71124b5430c71ee29872ccb2ba9a9c868a267f37
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116375"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/staffmembers/71d64d0e-7225-49b6-b0b1-070d476cda51"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphBookingStaffMember *bookingStaffMember = [[MSGraphBookingStaffMember alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```