---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 698f02dd591199d87d530b23dda1026c090291ac1c287b6bd86cb89257799cf8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278555"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphGroup *group = [[MSGraphGroup alloc] init];
[group setDescription:@"Group with designated owner and members"];
[group setDisplayName:@"Operations group"];
NSMutableArray *groupTypesList = [[NSMutableArray alloc] init];
[group setGroupTypes:groupTypesList];
[group setMailEnabled: false];
[group setMailNickname:@"operations2019"];
[group setSecurityEnabled: true];

NSError *error;
NSData *groupData = [group getSerializedDataWithError:&error];
[urlRequest setHTTPBody:groupData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```