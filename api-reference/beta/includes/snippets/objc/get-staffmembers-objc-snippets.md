---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f50bdfc022a0628524e0839dbfc9d4d6f9b2e99c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709699"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffMembers"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *bookingStaffMemberList = [[NSMutableArray alloc] init];
        bookingStaffMemberList = [jsonFinal valueForKey:@"value"];
        MSGraphBookingStaffMember *bookingStaffMember = [[MSGraphBookingStaffMember alloc] initWithDictionary:[bookingStaffMemberList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```