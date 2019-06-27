---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7b987c3a03b5bcf3122c4419be6e4ec99921e9dd
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35322761"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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