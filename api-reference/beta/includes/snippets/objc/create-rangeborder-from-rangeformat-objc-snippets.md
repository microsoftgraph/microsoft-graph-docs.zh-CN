---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ed029d593f051ef94ead25b97831500384cdd282a079d466131929e96361632
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163933"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/names/{name}/range/format/borders"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookRangeBorder *workbookRangeBorder = [[MSGraphWorkbookRangeBorder alloc] init];
[workbookRangeBorder setId:@"id-value"];
[workbookRangeBorder setColor:@"color-value"];
[workbookRangeBorder setStyle:@"style-value"];
[workbookRangeBorder setSideIndex:@"sideIndex-value"];
[workbookRangeBorder setWeight:@"weight-value"];

NSError *error;
NSData *workbookRangeBorderData = [workbookRangeBorder getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookRangeBorderData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```