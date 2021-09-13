---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dce96a5882ae3102cd224651549079173b3913c0963a22c0ec61efe55ca39cf7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162576"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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