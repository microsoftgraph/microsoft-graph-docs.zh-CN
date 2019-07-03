---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 67458ed48e7dcddcd72c1ecb98e456bc715f2381
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519798"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/names"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *workbookNamedItemList = [[NSMutableArray alloc] init];
        workbookNamedItemList = [jsonFinal valueForKey:@"value"];
        MSGraphWorkbookNamedItem *workbookNamedItem = [[MSGraphWorkbookNamedItem alloc] initWithDictionary:[workbookNamedItemList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```