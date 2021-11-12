---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 521037e840b6fee56522f5310ddada5472bea54fdaf254e482a5e5e767a86a34
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219824"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/{id|name}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookWorksheet *workbookWorksheet = [[MSGraphWorkbookWorksheet alloc] init];
[workbookWorksheet setPosition: 99];
[workbookWorksheet setName:@"name-value"];
[workbookWorksheet setVisibility:@"visibility-value"];

NSError *error;
NSData *workbookWorksheetData = [workbookWorksheet getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookWorksheetData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```