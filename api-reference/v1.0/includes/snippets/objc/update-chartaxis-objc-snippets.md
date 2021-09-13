---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8cd4610c8444e82e7a1db20a269e1feae130ec032dc83f4c58413ed391c5e6cd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218414"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis"]]];
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