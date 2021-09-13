---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4e8f426066258b0ecdc33b46362e6297a30de855930fde351076268346c944d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378699"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookTableColumn *workbookTableColumn = [[MSGraphWorkbookTableColumn alloc] init];
[workbookTableColumn setName:@"name-value"];
[workbookTableColumn setIndex: 99];
[workbookTableColumn setValues:@"values-value"];

NSError *error;
NSData *workbookTableColumnData = [workbookTableColumn getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookTableColumnData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```