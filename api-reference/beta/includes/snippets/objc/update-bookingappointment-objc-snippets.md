---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64d88c11026604cbe26dc5197cfc78e70dd2d05e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094839"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/appointments/AAMkADKnAAA="]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphBookingAppointment *bookingAppointment = [[MSGraphBookingAppointment alloc] init];
MSGraphDateTimeTimeZone *end = [[MSGraphDateTimeTimeZone alloc] init];
[end setDateTime: "2018-05-06T12:30:00+00:00"];
[end setTimeZone:@"UTC"];
[bookingAppointment setEnd:end];
MSGraphDateTimeTimeZone *invoiceDate = [[MSGraphDateTimeTimeZone alloc] init];
[invoiceDate setDateTime: "2018-05-06T12:30:00+00:00"];
[invoiceDate setTimeZone:@"UTC"];
[bookingAppointment setInvoiceDate:invoiceDate];
MSGraphDateTimeTimeZone *start = [[MSGraphDateTimeTimeZone alloc] init];
[start setDateTime: "2018-05-06T12:00:00+00:00"];
[start setTimeZone:@"UTC"];
[bookingAppointment setStart:start];

NSError *error;
NSData *bookingAppointmentData = [bookingAppointment getSerializedDataWithError:&error];
[urlRequest setHTTPBody:bookingAppointmentData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```