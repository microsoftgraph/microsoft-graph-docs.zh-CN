---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0519582268c64dc8312a149c4057ab18e1ff033d
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52871399"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk="]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphConversationMember *conversationMember = [[MSGraphConversationMember alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```