---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 277895eff1acbea2857a1636e697519bf4bdfd11
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616804"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites/{site-id}/lists"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphList *list = [[MSGraphList alloc] init];
[list setDisplayName:@"Books"];
NSMutableArray *columnsList = [[NSMutableArray alloc] init];
MSGraphColumnDefinition *columns = [[MSGraphColumnDefinition alloc] init];
[columns setName:@"Author"];
MSGraphTextColumn *text = [[MSGraphTextColumn alloc] init];
[columns setText:text];
[columnsList addObject: columns];
MSGraphColumnDefinition *columns = [[MSGraphColumnDefinition alloc] init];
[columns setName:@"PageCount"];
MSGraphNumberColumn *number = [[MSGraphNumberColumn alloc] init];
[columns setNumber:number];
[columnsList addObject: columns];
[list setColumns:columnsList];
MSGraphListInfo *list = [[MSGraphListInfo alloc] init];
[list setTemplate:@"genericList"];
[list setList:list];

NSError *error;
NSData *listData = [list getSerializedDataWithError:&error];
[urlRequest setHTTPBody:listData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```