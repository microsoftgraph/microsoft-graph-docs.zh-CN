---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee46821b5ddaba004874bd10b898fc177f487f17cbff3467faeaf5af37a8098c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163649"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/webAccounts"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWebAccount *webAccount = [[MSGraphWebAccount alloc] init];
[webAccount setDescription:@"My Github contributions!"];
[webAccount setUserId:@"innocenty.popov"];
MSGraphServiceInformation *service = [[MSGraphServiceInformation alloc] init];
[service setName:@"GitHub"];
[service setWebUrl:@"https://github.com"];
[webAccount setService:service];

NSError *error;
NSData *webAccountData = [webAccount getSerializedDataWithError:&error];
[urlRequest setHTTPBody:webAccountData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```