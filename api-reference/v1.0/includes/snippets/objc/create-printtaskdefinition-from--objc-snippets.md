---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8887470238fd6fb076f4ad7ae315282c3aaa0546
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772189"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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