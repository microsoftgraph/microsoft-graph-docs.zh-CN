---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21fd0546fdfcc51d95d3ea1710329d4e4bfe150bdd59706d93a67b11014f7f56
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158455"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{teamId}/schedule"]]];
[urlRequest setHTTPMethod:@"PUT"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSchedule *schedule = [[MSGraphSchedule alloc] init];
[schedule setEnabled: true];
[schedule setTimeZone:@"America/Chicago"];

NSError *error;
NSData *scheduleData = [schedule getSerializedDataWithError:&error];
[urlRequest setHTTPBody:scheduleData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```