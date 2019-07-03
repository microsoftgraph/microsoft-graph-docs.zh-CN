---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 39ac44d1374a7d124e9134090e8428dde89556e9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35510066"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/names/{name}/range/format/protection"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookFormatProtection *workbookFormatProtection = [[MSGraphWorkbookFormatProtection alloc] init];
[workbookFormatProtection setLocked: true];
[workbookFormatProtection setFormulaHidden: true];

NSError *error;
NSData *workbookFormatProtectionData = [workbookFormatProtection getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookFormatProtectionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```