---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54f363ebf8473593d3778e2b09c4f13f3e28d459779ee5ec1d6d3beab4e9dfba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378640"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{teamId}/schedule/timesOff?$filter=sharedTimeOff/startDateTime%20ge%202019-03-11T00:00:00.000Z%20and%20sharedTimeOff/endDateTime%20le%202019-03-18T00:00:00.000Z%20and%20draftTimeOff/startDateTime%20ge%202019-03-11T00:00:00.000Z%20and%20draftTimeOff/endDateTime%20le%202019-03-18T00:00:00.000Z"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        MSCollection *collection = [[MSCollection alloc] initWithData:data error:&jsonError];
        MSGraphTimeOff *timeOff = [[MSGraphTimeOff alloc] initWithDictionary:[[collection value] objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```