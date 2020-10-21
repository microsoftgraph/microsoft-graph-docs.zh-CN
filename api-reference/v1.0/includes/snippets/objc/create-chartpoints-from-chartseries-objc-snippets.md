---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab7c1dfe5e6a16acad2b70dc342fd705a695e2cb
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614345"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookChartPoint *workbookChartPoint = [[MSGraphWorkbookChartPoint alloc] init];

NSError *error;
NSData *workbookChartPointData = [workbookChartPoint getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookChartPointData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```