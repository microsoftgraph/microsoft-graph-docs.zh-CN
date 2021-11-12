---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d15d5ed6e328a88c847e901d84d46677b945c3c6fbc7e4831ed2725ebd38fba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277815"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookChartSeries *workbookChartSeries = [[MSGraphWorkbookChartSeries alloc] init];
[workbookChartSeries setName:@"name-value"];

NSError *error;
NSData *workbookChartSeriesData = [workbookChartSeries getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookChartSeriesData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```