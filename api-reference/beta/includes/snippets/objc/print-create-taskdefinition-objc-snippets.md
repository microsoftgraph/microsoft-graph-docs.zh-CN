---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37291be92d077240b53fc40a3d54ee72439d0cbc89a1d788779dee2ed7d6ddb1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333091"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/print/taskDefinitions"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPrintTaskDefinition *printTaskDefinition = [[MSGraphPrintTaskDefinition alloc] init];
[printTaskDefinition setDisplayName:@"Test TaskDefinitionName"];
MSGraphAppIdentity *createdBy = [[MSGraphAppIdentity alloc] init];
[createdBy setDisplayName:@"Requesting App Display Name"];
[printTaskDefinition setCreatedBy:createdBy];

NSError *error;
NSData *printTaskDefinitionData = [printTaskDefinition getSerializedDataWithError:&error];
[urlRequest setHTTPBody:printTaskDefinitionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```