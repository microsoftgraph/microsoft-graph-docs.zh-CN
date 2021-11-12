---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 279d2638090c7a9671352baada30973538acc08a5422d340ec763275ab116059
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904031"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
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