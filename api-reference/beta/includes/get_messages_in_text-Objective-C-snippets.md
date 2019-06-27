---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a1265caba59533badb1c92bd2a31b9b69f577ddb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35318504"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/messages?$select=subject,body,bodyPreview,uniqueBody"]]];
[urlRequest setHTTPMethod:@"GET"];
[urlRequest setValue:@"outlook.body-content-type=\"text\"" forHTTPHeaderField:@"Prefer"];

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