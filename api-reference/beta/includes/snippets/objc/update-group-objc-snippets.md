---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a993408b6c53ee3eda4b8dbcb60b03e6787b6188
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711715"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphGroup *group = [[MSGraphGroup alloc] init];
[group setDescription:@"description-value"];
[group setDisplayName:@"displayName-value"];
NSMutableArray *groupTypesList = [[NSMutableArray alloc] init];
[groupTypesList addObject: @"groupTypes-value"];
[group setGroupTypes:groupTypesList];
[group setMail:@"mail-value"];
[group setMailEnabled: true];
[group setMailNickname:@"mailNickname-value"];

NSError *error;
NSData *groupData = [group getSerializedDataWithError:&error];
[urlRequest setHTTPBody:groupData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```