---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b58a4e0b5e3c3af30a8640186c2b25e686da54ca16659282ae4c6554cb56a2e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106831"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookChartLineFormat *workbookChartLineFormat = [[MSGraphWorkbookChartLineFormat alloc] init];
[workbookChartLineFormat setColor:@"color-value"];

NSError *error;
NSData *workbookChartLineFormatData = [workbookChartLineFormat getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookChartLineFormatData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```