---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ed263a4f43eda0c2c212067c8558f70fcbd2301
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691101"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members?$filter=(microsoft.graph.aadUserConversationMember/displayName%20eq%20'Harry%20Johnson'%20or%20microsoft.graph.aadUserConversationMember/email%20eq%20'admin@M365x987948.OnMicrosoft.com')"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        MSCollection *collection = [[MSCollection alloc] initWithData:data error:&jsonError];
        MSGraphConversationMember *conversationMember = [[MSGraphConversationMember alloc] initWithDictionary:[[collection value] objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```