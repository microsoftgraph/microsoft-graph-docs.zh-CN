---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37b8dad49d019ae0f627a8fb44accb8c65e31c7e6cbe7ae39ff99141f925cb03
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101389"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'123456789'"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        MSCollection *collection = [[MSCollection alloc] initWithData:data error:&jsonError];
        MSGraphOnlineMeeting *onlineMeeting = [[MSGraphOnlineMeeting alloc] initWithDictionary:[[collection value] objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```