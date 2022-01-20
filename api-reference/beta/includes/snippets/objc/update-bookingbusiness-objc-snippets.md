---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ec4f6d356495bbd863e7db37471fca79a69782a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129990"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/bookingBusinesses/fabrikam@contoso.onmicrosoft.com"]]];
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