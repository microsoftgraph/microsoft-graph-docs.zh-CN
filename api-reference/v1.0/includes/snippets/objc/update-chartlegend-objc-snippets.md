---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 724982152271bbd543300f26e4fa3ec660f835befdf1838a9fe1e07439186cf5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163863"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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