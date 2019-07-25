---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4ec6e8bfa0e47c977df278991b7d0bfb1727c56b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708019"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *workbookChartPointList = [[NSMutableArray alloc] init];
        workbookChartPointList = [jsonFinal valueForKey:@"value"];
        MSGraphWorkbookChartPoint *workbookChartPoint = [[MSGraphWorkbookChartPoint alloc] initWithDictionary:[workbookChartPointList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```