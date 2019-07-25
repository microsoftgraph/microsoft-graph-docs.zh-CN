---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d1c0842f2362e72594c9ec6a53d298e672127963
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727774"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/names/{name}/range/format/borders"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *workbookRangeBorderList = [[NSMutableArray alloc] init];
        workbookRangeBorderList = [jsonFinal valueForKey:@"value"];
        MSGraphWorkbookRangeBorder *workbookRangeBorder = [[MSGraphWorkbookRangeBorder alloc] initWithDictionary:[workbookRangeBorderList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```