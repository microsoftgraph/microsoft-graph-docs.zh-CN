---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fb9561cb34c2bb1aa39d2774257fc749b2941d28bc49bcb799001eefc321b13
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162281"
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