---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2e33b7153ed71b51a6d0f35e6fac4780dc696d3
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613111"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookChartLegend *workbookChartLegend = [[MSGraphWorkbookChartLegend alloc] init];
[workbookChartLegend setVisible: true];
[workbookChartLegend setPosition:@"position-value"];
[workbookChartLegend setOverlay: true];

NSError *error;
NSData *workbookChartLegendData = [workbookChartLegend getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookChartLegendData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```