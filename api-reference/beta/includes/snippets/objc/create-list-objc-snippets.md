---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e869c2c0f5a1438b2b242e336a74454d4fd1e1344713af5ca699f489e7b0c432
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277427"
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