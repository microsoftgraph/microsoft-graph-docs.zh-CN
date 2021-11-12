---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffcf67ab1f2135bc4482e733d8ea01846d23553af1cdd7627fb5098b68b30909
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215881"
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