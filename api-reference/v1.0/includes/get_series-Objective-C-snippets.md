---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b1d66375f17887863eab6e478c886850f47961da
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35314503"
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