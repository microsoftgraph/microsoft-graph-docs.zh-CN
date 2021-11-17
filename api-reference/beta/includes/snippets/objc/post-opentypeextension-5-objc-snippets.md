---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e335d787c2e13ae7bc824eb09e04ee9baf1315ddaa5e8226a50d264f83ce8f2e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333146"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/conversations"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphConversation *conversation = [[MSGraphConversation alloc] init];
[conversation setTopic:@"Does anyone have a second?"];
NSMutableArray *ThreadsList = [[NSMutableArray alloc] init];
MSGraphConversationThread *Threads = [[MSGraphConversationThread alloc] init];
NSMutableArray *PostsList = [[NSMutableArray alloc] init];
MSGraphPost *Posts = [[MSGraphPost alloc] init];
MSGraphItemBody *Body = [[MSGraphItemBody alloc] init];
[Body setContentType: [MSGraphBodyType html]];
[Body setContent:@"This is urgent!"];
[Posts setBody:Body];
NSMutableArray *ExtensionsList = [[NSMutableArray alloc] init];
MSGraphExtension *Extensions = [[MSGraphExtension alloc] init];
[Extensions setExtensionName:@"Com.Contoso.Benefits"];
[Extensions setCompanyName:@"Contoso"];
[Extensions setExpirationDate: "2016-08-03T11:00:00Z"];
NSMutableArray *topPicksList = [[NSMutableArray alloc] init];
[topPicksList addObject: @"Employees only"];
[topPicksList addObject: @"Add spouse or guest"];
[topPicksList addObject: @"Add family"];
[Extensions setTopPicks:topPicksList];
[ExtensionsList addObject: Extensions];
[Posts setExtensions:ExtensionsList];
[PostsList addObject: Posts];
[Threads setPosts:PostsList];
[ThreadsList addObject: Threads];
[conversation setThreads:ThreadsList];

NSError *error;
NSData *conversationData = [conversation getSerializedDataWithError:&error];
[urlRequest setHTTPBody:conversationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```