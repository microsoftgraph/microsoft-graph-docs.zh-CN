---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 31405e5c46a81ccd85d5c29b395adcec6ccce348
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35323296"
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