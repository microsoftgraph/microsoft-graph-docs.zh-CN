---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04afa80763a9ef1be08245da6f7b17b17a78d9a2
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212428"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/organization/{organizationId}/settings/microsoftApplicationDataAccess"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphMicrosoftApplicationDataAccessSettings *microsoftApplicationDataAccessSettings = [[MSGraphMicrosoftApplicationDataAccessSettings alloc] init];
[microsoftApplicationDataAccessSettings setDisabledForGroup:@"edbfe4fb-ec70-4300-928f-dbb2ae86c981"];

NSError *error;
NSData *microsoftApplicationDataAccessSettingsData = [microsoftApplicationDataAccessSettings getSerializedDataWithError:&error];
[urlRequest setHTTPBody:microsoftApplicationDataAccessSettingsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```