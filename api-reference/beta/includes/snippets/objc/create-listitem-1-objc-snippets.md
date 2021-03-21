---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a980c3a9022e75a2d3e92b5dfa4d254635f72afa
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957958"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites/{site-id}/lists/{list-id}/items"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphListItem *listItem = [[MSGraphListItem alloc] init];
MSGraphFieldValueSet *fields = [[MSGraphFieldValueSet alloc] init];
[fields setTitle:@"Widget"];
[fields setColor:@"Purple"];
[fields setWeight: 32];
[listItem setFields:fields];

NSError *error;
NSData *listItemData = [listItem getSerializedDataWithError:&error];
[urlRequest setHTTPBody:listItemData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```