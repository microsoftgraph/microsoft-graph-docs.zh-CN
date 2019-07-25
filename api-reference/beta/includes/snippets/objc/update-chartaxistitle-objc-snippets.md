---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f8a6e45ec73440501fdafda1ae45771cc1b5d9a0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708306"
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