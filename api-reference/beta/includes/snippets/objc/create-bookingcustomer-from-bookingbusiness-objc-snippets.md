---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4e4c379bd68a59d7e997be4749d116d34a4b89e78ab1d69a2a099732aff61a9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105045"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphBookingCustomer *bookingCustomer = [[MSGraphBookingCustomer alloc] init];
[bookingCustomer setDisplayName:@"Joni Sherman"];
[bookingCustomer setEmailAddress:@"jonis@relecloud.com"];

NSError *error;
NSData *bookingCustomerData = [bookingCustomer getSerializedDataWithError:&error];
[urlRequest setHTTPBody:bookingCustomerData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```