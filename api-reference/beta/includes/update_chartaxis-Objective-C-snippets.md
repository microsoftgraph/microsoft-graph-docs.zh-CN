---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ab2b68a1f719a396f1990ea68dd8501fae623f5b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35318114"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookChartAxis *workbookChartAxis = [[MSGraphWorkbookChartAxis alloc] init];
MSGraphJson *majorUnit = [[MSGraphJson alloc] init];
[workbookChartAxis setMajorUnit:majorUnit];
MSGraphJson *maximum = [[MSGraphJson alloc] init];
[workbookChartAxis setMaximum:maximum];
MSGraphJson *minimum = [[MSGraphJson alloc] init];
[workbookChartAxis setMinimum:minimum];

NSError *error;
NSData *workbookChartAxisData = [workbookChartAxis getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookChartAxisData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```