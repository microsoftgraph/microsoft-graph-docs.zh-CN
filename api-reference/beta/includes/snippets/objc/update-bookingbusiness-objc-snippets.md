---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45698a90829addfcd2c1ed7288fed5a58b495348a866234f70ba783850db7a74
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105039"
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