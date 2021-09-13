---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a51e23230bfc8b96ad35b75259559a82106ca1c6c787f007fa4212875ca3892
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158401"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{teamId}/schedule/share"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

BOOL notifyTeam = YES;
payloadDictionary[@"notifyTeam"] = notifyTeam;

NSString *startDateTimeDateTimeString = @"10/08/2018 00:00:00";
NSDate *startDateTime = [NSDate ms_dateFromString: startDateTimeDateTimeString];
payloadDictionary[@"startDateTime"] = startDateTime;

NSString *endDateTimeDateTimeString = @"10/15/2018 00:00:00";
NSDate *endDateTime = [NSDate ms_dateFromString: endDateTimeDateTimeString];
payloadDictionary[@"endDateTime"] = endDateTime;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```