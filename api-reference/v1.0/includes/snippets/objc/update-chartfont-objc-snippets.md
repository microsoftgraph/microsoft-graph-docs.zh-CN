---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f574d6f20d62bb8b1c3dc7a45e20ce1441100eb08386ae6bab4f1c41f76c7d7f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163531"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookChartFont *workbookChartFont = [[MSGraphWorkbookChartFont alloc] init];
[workbookChartFont setBold: true];
[workbookChartFont setColor:@"color-value"];
[workbookChartFont setItalic: true];
[workbookChartFont setName:@"name-value"];
[workbookChartFont setSize: 99];
[workbookChartFont setUnderline:@"underline-value"];

NSError *error;
NSData *workbookChartFontData = [workbookChartFont getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookChartFontData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```