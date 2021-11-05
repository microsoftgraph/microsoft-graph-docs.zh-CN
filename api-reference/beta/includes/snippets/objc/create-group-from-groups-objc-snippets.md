---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04c0a2863d51b98a8f10451a5595fd10ba4d30b4
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780506"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups/$ref"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphGroup *group = [[MSGraphGroup alloc] init];

NSError *error;
NSData *groupData = [group getSerializedDataWithError:&error];
[urlRequest setHTTPBody:groupData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```