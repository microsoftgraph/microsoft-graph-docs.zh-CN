---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a14acbee82771dfcbe5825cea44697ccc7fecce1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706655"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directoryRoles"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphDirectoryRole *directoryRole = [[MSGraphDirectoryRole alloc] init];
[directoryRole setDescription:@"description-value"];
[directoryRole setDisplayName:@"displayName-value"];
[directoryRole setRoleTemplateId:@"roleTemplateId-value"];

NSError *error;
NSData *directoryRoleData = [directoryRole getSerializedDataWithError:&error];
[urlRequest setHTTPBody:directoryRoleData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```