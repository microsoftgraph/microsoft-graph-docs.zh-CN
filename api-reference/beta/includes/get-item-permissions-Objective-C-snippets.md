---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c3c2b67b4cd868a43fe1ec11ddeeb05e3ae9ba96
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330117"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{item-id}/permissions"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *permissionList = [[NSMutableArray alloc] init];
        permissionList = [jsonFinal valueForKey:@"value"];
        MSGraphPermission *permission = [[MSGraphPermission alloc] initWithDictionary:[permissionList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```