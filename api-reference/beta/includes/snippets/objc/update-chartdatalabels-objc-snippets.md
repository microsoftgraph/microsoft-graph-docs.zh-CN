---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e4d9f0e9d4819c0fa0d2164055ef27e30c6d9f4c04a5e7d0511a17facdaef9d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158559"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/datalabels"]]];
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