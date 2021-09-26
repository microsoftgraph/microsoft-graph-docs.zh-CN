---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b03b66a01b063ad3862fbdad038c40e9d2039369
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763868"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ/workbook/tables/Table1/rows"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"respond-async" forHTTPHeaderField:@"Prefer"];
[urlRequest setValue:@"{Workbook-Session-Id}" forHTTPHeaderField:@"Workbook-Session-Id"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookTableRow *workbookTableRow = [[MSGraphWorkbookTableRow alloc] init];
[workbookTableRow setValues:@"[\r\n    [1, 2, 3],\r\n    [4, 5, 6]\r\n  ]"];

NSError *error;
NSData *workbookTableRowData = [workbookTableRow getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookTableRowData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```