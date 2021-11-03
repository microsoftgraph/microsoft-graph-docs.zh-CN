---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f61721adda9c349236805ff75f539b37d76611f466461559f38fcaf802cf30be
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278346"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphColumnDefinition *columnDefinition = [[MSGraphColumnDefinition alloc] init];
[columnDefinition setRequired: true];
[columnDefinition setHidden: false];
[columnDefinition setPropagateChanges: false];

NSError *error;
NSData *columnDefinitionData = [columnDefinition getSerializedDataWithError:&error];
[urlRequest setHTTPBody:columnDefinitionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```