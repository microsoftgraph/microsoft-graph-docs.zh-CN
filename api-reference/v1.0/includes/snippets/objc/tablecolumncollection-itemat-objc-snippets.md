---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a840b878630cd12db5921e3564b6bca1981c0e22
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493554"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/tables/{id|name}/columns/itemAt"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookTableColumn *workbookTableColumn = [[MSGraphWorkbookTableColumn alloc] init];
[workbookTableColumn setIndex: 3];

NSError *error;
NSData *workbookTableColumnData = [workbookTableColumn getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookTableColumnData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```