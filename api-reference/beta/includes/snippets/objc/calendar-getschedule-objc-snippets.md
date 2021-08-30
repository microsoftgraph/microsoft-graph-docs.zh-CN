---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 750baa40a9a6b4b76012bccbc27a058c792af6be82c6037c8c2f8dd64403e415
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215898"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/calendar/getSchedule"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"outlook.timezone=\"Pacific Standard Time\"" forHTTPHeaderField:@"Prefer"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *schedulesList = [[NSMutableArray alloc] init];
[schedulesList addObject: @"adelev@contoso.onmicrosoft.com"];
[schedulesList addObject: @"meganb@contoso.onmicrosoft.com"];
payloadDictionary[@"schedules"] = schedulesList;

MSGraphDateTimeTimeZone *startTime = [[MSGraphDateTimeTimeZone alloc] init];
[startTime setDateTime: "2019-03-15T09:00:00"];
[startTime setTimeZone:@"Pacific Standard Time"];
payloadDictionary[@"startTime"] = startTime;

MSGraphDateTimeTimeZone *endTime = [[MSGraphDateTimeTimeZone alloc] init];
[endTime setDateTime: "2019-03-15T18:00:00"];
[endTime setTimeZone:@"Pacific Standard Time"];
payloadDictionary[@"endTime"] = endTime;

int32_t availabilityViewInterval = 60;
payloadDictionary[@"availabilityViewInterval"] = availabilityViewInterval;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```