---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c8ad62603a5799e9b725eed94f8447cba47234e1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35323318"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *workbookTableColumnList = [[NSMutableArray alloc] init];
        workbookTableColumnList = [jsonFinal valueForKey:@"value"];
        MSGraphWorkbookTableColumn *workbookTableColumn = [[MSGraphWorkbookTableColumn alloc] initWithDictionary:[workbookTableColumnList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```