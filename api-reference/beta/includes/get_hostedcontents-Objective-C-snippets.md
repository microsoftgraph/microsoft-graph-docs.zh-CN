---
description: 自动生成的文件。 不修改
ms.openlocfilehash: eda0abba23bfcd2376b7ca8e9b9da1cc1c45a118
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330464"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/chats/{id}/messages/{id}/hostedContents"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *chatMessageHostedContentList = [[NSMutableArray alloc] init];
        chatMessageHostedContentList = [jsonFinal valueForKey:@"value"];
        MSGraphChatMessageHostedContent *chatMessageHostedContent = [[MSGraphChatMessageHostedContent alloc] initWithDictionary:[chatMessageHostedContentList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```