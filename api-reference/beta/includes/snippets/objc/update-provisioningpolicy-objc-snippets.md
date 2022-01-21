---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62c6dd30ea5af74495218dbda5bd1e3213c7b131
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131442"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/deviceManagement/virtualEndpoint/provisioningPolicies/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphCloudPcProvisioningPolicy *cloudPcProvisioningPolicy = [[MSGraphCloudPcProvisioningPolicy alloc] init];
[cloudPcProvisioningPolicy setDisplayName:@"HR provisioning policy"];
[cloudPcProvisioningPolicy setDescription:@"Provisioning policy for India HR employees"];
[cloudPcProvisioningPolicy setOnPremisesConnectionId:@"4e47d0f6-6f77-44f0-8893-c0fe1701b553"];

NSError *error;
NSData *cloudPcProvisioningPolicyData = [cloudPcProvisioningPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:cloudPcProvisioningPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```