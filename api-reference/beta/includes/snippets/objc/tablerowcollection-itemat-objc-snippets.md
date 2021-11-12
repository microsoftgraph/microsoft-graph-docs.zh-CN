---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff8ebd62e2e9d6573c34be36dc8d353b52646992e97ecbbe2fb85b7edcbada3d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162717"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/tables/{id|name}/rows/ItemAt"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookTableRow *workbookTableRow = [[MSGraphWorkbookTableRow alloc] init];
MSGraphInt32 *index = [[MSGraphInt32 alloc] init];
[workbookTableRow setIndex:index];

NSError *error;
NSData *workbookTableRowData = [workbookTableRow getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookTableRowData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```