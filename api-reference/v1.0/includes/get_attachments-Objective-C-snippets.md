---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 49c287789177f10a8ad06b4200d8edfd640c4597
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35323324"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/{id}/threads/{id}/posts/{id}/attachments"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *attachmentList = [[NSMutableArray alloc] init];
        attachmentList = [jsonFinal valueForKey:@"value"];
        MSGraphAttachment *attachment = [[MSGraphAttachment alloc] initWithDictionary:[attachmentList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```