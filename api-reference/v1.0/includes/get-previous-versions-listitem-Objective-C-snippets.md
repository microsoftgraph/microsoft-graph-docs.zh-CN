---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9c95b5c39a5d1d7129423e7bb9186a1bb2b7a835
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35314596"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites/{site-id}/lists/{list-id}/items/{item-id}/versions"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *listItemVersionList = [[NSMutableArray alloc] init];
        listItemVersionList = [jsonFinal valueForKey:@"value"];
        MSGraphListItemVersion *listItemVersion = [[MSGraphListItemVersion alloc] initWithDictionary:[listItemVersionList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```