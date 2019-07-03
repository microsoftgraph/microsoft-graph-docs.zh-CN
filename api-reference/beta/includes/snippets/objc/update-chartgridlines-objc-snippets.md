---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5ea509068a294280df8a256d242b0918112b428d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478806"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/minorgridlines"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookChartGridlines *workbookChartGridlines = [[MSGraphWorkbookChartGridlines alloc] init];
[workbookChartGridlines setVisible: true];

NSError *error;
NSData *workbookChartGridlinesData = [workbookChartGridlines getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookChartGridlinesData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```