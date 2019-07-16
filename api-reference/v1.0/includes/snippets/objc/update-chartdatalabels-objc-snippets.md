---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 80d3021f1ee762cd1f97172c30559d2da5c73198
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737343"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/dataLabels"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookChartDataLabels *workbookChartDataLabels = [[MSGraphWorkbookChartDataLabels alloc] init];
[workbookChartDataLabels setPosition:@"position-value"];
[workbookChartDataLabels setShowValue: true];
[workbookChartDataLabels setShowSeriesName: true];
[workbookChartDataLabels setShowCategoryName: true];
[workbookChartDataLabels setShowLegendKey: true];

NSError *error;
NSData *workbookChartDataLabelsData = [workbookChartDataLabels getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookChartDataLabelsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```