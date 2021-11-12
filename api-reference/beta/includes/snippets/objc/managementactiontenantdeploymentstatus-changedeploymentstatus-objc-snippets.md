---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7d35b530775305ae3aa31658a47c071b1bc161c4a16c37bf2760d673296d0fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219444"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/changeDeploymentStatus"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSString *tenantGroupId = @"String";
payloadDictionary[@"tenantGroupId"] = tenantGroupId;

NSString *tenantId = @"String";
payloadDictionary[@"tenantId"] = tenantId;

NSString *managementActionId = @"String";
payloadDictionary[@"managementActionId"] = managementActionId;

NSString *managementTemplateId = @"String";
payloadDictionary[@"managementTemplateId"] = managementTemplateId;

NSString *status = @"String";
payloadDictionary[@"status"] = status;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```