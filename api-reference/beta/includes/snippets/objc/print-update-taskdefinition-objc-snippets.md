---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0af567e990dcc25688eb9bd8fedd3ef3c3546e4ae6e612219f746e0c1cc952d7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332874"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/print/taskDefinitions/fab143fd-ee61-4358-8558-2c7dee953982"]]];
[urlRequest setHTTPMethod:@"PATCH"];
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