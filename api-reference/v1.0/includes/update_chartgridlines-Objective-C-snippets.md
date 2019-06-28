---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2f0b829b2b14c05c6f976dcb50e60a8170c1fac7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35323217"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines"]]];
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