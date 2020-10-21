---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f17bb9a57908e51e3c4677ccb3791fd7c219f8c3
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609111"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/protect"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

MSGraphWorkbookWorksheetProtectionOptions *options = [[MSGraphWorkbookWorksheetProtectionOptions alloc] init];
[options setAllowFormatCells: true];
[options setAllowFormatColumns: true];
[options setAllowFormatRows: true];
[options setAllowInsertColumns: true];
[options setAllowInsertRows: true];
[options setAllowInsertHyperlinks: true];
[options setAllowDeleteColumns: true];
[options setAllowDeleteRows: true];
[options setAllowSort: true];
[options setAllowAutoFilter: true];
[options setAllowPivotTables: true];
payloadDictionary[@"options"] = options;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```