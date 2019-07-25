---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fe35af2150fb7ff78d0c7672d109c736bf09139e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724848"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *workbookTableRowList = [[NSMutableArray alloc] init];
        workbookTableRowList = [jsonFinal valueForKey:@"value"];
        MSGraphWorkbookTableRow *workbookTableRow = [[MSGraphWorkbookTableRow alloc] initWithDictionary:[workbookTableRowList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```