---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 348a6d59af8e97b5c6582f4c414e5f081caf6cb3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740409"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/root/workbook/worksheets/{id}/pivotTables"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *workbookPivotTableList = [[NSMutableArray alloc] init];
        workbookPivotTableList = [jsonFinal valueForKey:@"value"];
        MSGraphWorkbookPivotTable *workbookPivotTable = [[MSGraphWorkbookPivotTable alloc] initWithDictionary:[workbookPivotTableList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```