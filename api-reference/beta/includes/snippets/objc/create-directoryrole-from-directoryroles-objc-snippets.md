---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c884e41c47020218e355584815814b68e223d964d026179f11bd061e3e19b16
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277806"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directoryRoles"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphDirectoryRole *directoryRole = [[MSGraphDirectoryRole alloc] init];
[directoryRole setRoleTemplateId:@"fe930be7-5e62-47db-91af-98c3a49a38b1"];

NSError *error;
NSData *directoryRoleData = [directoryRole getSerializedDataWithError:&error];
[urlRequest setHTTPBody:directoryRoleData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```