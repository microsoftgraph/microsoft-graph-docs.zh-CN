---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8ae4800a78a45a3fa6a3ae401f76afb68bb393f6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729935"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
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