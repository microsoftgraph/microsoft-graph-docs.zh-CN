---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4024fb6e41419515d87a699214dd1f1ac59e9b48
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608105"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphBookingBusiness *bookingBusiness = [[MSGraphBookingBusiness alloc] init];
[bookingBusiness setEmail:@"admin@fabrikam.com"];
MSGraphBookingSchedulingPolicy *schedulingPolicy = [[MSGraphBookingSchedulingPolicy alloc] init];
[schedulingPolicy setTimeSlotInterval:@"PT60M"];
[schedulingPolicy setMinimumLeadTime:@"P1D"];
[schedulingPolicy setMaximumAdvance:@"P30D"];
[schedulingPolicy setSendConfirmationsToOwner: true];
[schedulingPolicy setAllowStaffSelection: true];
[bookingBusiness setSchedulingPolicy:schedulingPolicy];

NSError *error;
NSData *bookingBusinessData = [bookingBusiness getSerializedDataWithError:&error];
[urlRequest setHTTPBody:bookingBusinessData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```