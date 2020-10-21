---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eaf47fd5d6c61b4b85e31b74fab7b957fe8d9f4a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614901"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/outlook/masterCategories/bac262b7-485d-4739-b436-e31467d64fac"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOutlookCategory *outlookCategory = [[MSGraphOutlookCategory alloc] init];
[outlookCategory setColor: [MSGraphCategoryColor preset15]];

NSError *error;
NSData *outlookCategoryData = [outlookCategory getSerializedDataWithError:&error];
[urlRequest setHTTPBody:outlookCategoryData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```