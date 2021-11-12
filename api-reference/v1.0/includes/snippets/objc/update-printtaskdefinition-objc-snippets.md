---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 804b9ac923b1ae0e7cb3468968086919ca5b0f16c056f323318e241ce30b8cdd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902240"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/print/taskDefinitions/{printTaskDefinitionId}"]]];
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