---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c47120a9640f7f434cb03398600babbbb0af0d21ba22e382c32d8d8248a6b56a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163853"
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