---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93b6896591eadf4ab4122952dd802ec03648b3c1
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44218493"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{teamId}/schedule/shifts?$filter=sharedShift/startDateTime%20ge%202019-03-11T00:00:00.000Z%20and%20sharedShift/endDateTime%20le%202019-03-18T00:00:00.000Z%20and%20draftShift/startDateTime%20ge%202019-03-11T00:00:00.000Z%20and%20draftShift/endDateTime%20le%202019-03-18T00:00:00.000Z"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        MSCollection *collection = [[MSCollection alloc] initWithData:data error:&jsonError];
        MSGraphShift *shift = [[MSGraphShift alloc] initWithDictionary:[[collection value] objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```