---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bbd589495cc05953a6fb2486d6aae42e059d5ac
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609013"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/names/{name}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookNamedItem *workbookNamedItem = [[MSGraphWorkbookNamedItem alloc] init];
[workbookNamedItem setType:@"type-value"];
[workbookNamedItem setScope:@"scope-value"];
[workbookNamedItem setComment:@"comment-value"];
MSGraphJson *value = [[MSGraphJson alloc] init];
[workbookNamedItem setValue:value];
[workbookNamedItem setVisible: true];

NSError *error;
NSData *workbookNamedItemData = [workbookNamedItem getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookNamedItemData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```