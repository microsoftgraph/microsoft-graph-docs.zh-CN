---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd90c3c14e4acdf60ab8805d3d342500d5efb0757cef434688e18ea6ec3c496f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162383"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/names/{name}/range/format/fill"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookRangeFill *workbookRangeFill = [[MSGraphWorkbookRangeFill alloc] init];
[workbookRangeFill setColor:@"color-value"];

NSError *error;
NSData *workbookRangeFillData = [workbookRangeFill getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookRangeFillData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```