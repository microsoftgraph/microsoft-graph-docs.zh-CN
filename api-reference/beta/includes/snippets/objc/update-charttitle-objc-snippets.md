---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a9128e82aa8cc4d269106e0c0ec6f8ae005d908
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604901"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookChartTitle *workbookChartTitle = [[MSGraphWorkbookChartTitle alloc] init];
[workbookChartTitle setOverlay: true];
[workbookChartTitle setText:@"text-value"];
[workbookChartTitle setVisible: true];

NSError *error;
NSData *workbookChartTitleData = [workbookChartTitle getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookChartTitleData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```