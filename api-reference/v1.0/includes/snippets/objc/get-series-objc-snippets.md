---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b1d66375f17887863eab6e478c886850f47961da
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734144"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *workbookChartSeriesList = [[NSMutableArray alloc] init];
        workbookChartSeriesList = [jsonFinal valueForKey:@"value"];
        MSGraphWorkbookChartSeries *workbookChartSeries = [[MSGraphWorkbookChartSeries alloc] initWithDictionary:[workbookChartSeriesList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```