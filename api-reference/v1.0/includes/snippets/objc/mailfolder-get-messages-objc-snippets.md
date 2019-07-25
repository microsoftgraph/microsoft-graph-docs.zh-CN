---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6b7c120199e9c91b101cb4a4ce4a7bf4fc4aa14
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856452"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/mailFolders/{id}/messages"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *messageList = [[NSMutableArray alloc] init];
        messageList = [jsonFinal valueForKey:@"value"];
        MSGraphMessage *message = [[MSGraphMessage alloc] initWithDictionary:[messageList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```