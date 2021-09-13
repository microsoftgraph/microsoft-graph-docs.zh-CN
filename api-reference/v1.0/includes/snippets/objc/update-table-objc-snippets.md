---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17d90d8c97c1ea8a0194b6bb1718272ff924a58e7b31c159a7a5439dda178c7d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332424"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/tables/{id|name}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookTable *workbookTable = [[MSGraphWorkbookTable alloc] init];
[workbookTable setName:@"name-value"];
[workbookTable setShowHeaders: true];
[workbookTable setShowTotals: true];
[workbookTable setStyle:@"style-value"];

NSError *error;
NSData *workbookTableData = [workbookTable getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookTableData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```