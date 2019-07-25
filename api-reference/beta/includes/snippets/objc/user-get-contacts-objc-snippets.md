---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c1522c53678171d33ae5253079c9a157743eace8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867372"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/contacts?$select=displayName,emailAddresses"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *contactList = [[NSMutableArray alloc] init];
        contactList = [jsonFinal valueForKey:@"value"];
        MSGraphContact *contact = [[MSGraphContact alloc] initWithDictionary:[contactList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```