---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba6a9294c3a2a1dee55780b75c55d68c8d7a296a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613708"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookTableRow *workbookTableRow = [[MSGraphWorkbookTableRow alloc] init];
[workbookTableRow setIndex: 99];
[workbookTableRow setValues:@"values-value"];

NSError *error;
NSData *workbookTableRowData = [workbookTableRow getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookTableRowData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```