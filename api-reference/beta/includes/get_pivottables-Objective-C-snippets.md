---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 35aaa88c9d2b6446a1f2c64d0fbd965b2db7135e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35315574"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/drive/root/workbook/worksheets/{id}/pivotTables"]]];
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