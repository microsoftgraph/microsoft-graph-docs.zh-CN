---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f8a6e45ec73440501fdafda1ae45771cc1b5d9a0
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615385"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/title"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookChartAxisTitle *workbookChartAxisTitle = [[MSGraphWorkbookChartAxisTitle alloc] init];
[workbookChartAxisTitle setText:@"text-value"];
[workbookChartAxisTitle setVisible: true];

NSError *error;
NSData *workbookChartAxisTitleData = [workbookChartAxisTitle getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookChartAxisTitleData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```