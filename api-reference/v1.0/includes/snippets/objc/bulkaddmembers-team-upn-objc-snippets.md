---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4134af973439dbe04fe95620588ab989715305a7
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688408"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/e4183b04-c9a2-417c-bde4-70e3ee46a6dc/members/add"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *valuesList = [[NSMutableArray alloc] init];
MSGraphConversationMember *values = [[MSGraphConversationMember alloc] init];
NSMutableArray *rolesList = [[NSMutableArray alloc] init];
[values setRoles:rolesList];
[valuesList addObject: values];
MSGraphConversationMember *values = [[MSGraphConversationMember alloc] init];
NSMutableArray *rolesList = [[NSMutableArray alloc] init];
[rolesList addObject: @"owner"];
[values setRoles:rolesList];
[valuesList addObject: values];
payloadDictionary[@"values"] = valuesList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```