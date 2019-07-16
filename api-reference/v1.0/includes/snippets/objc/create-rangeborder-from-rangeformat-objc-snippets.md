---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c4e6aa5f35ee5551e5d60ef03759bb7b7e3b7ced
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740115"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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