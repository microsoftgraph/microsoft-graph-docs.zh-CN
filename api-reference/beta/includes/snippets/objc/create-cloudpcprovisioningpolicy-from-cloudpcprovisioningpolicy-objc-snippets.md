---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb705e320baca323a927e7dd2de08745f616a8ed
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089053"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/deviceManagement/virtualEndpoint/provisioningPolicies"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphCloudPcProvisioningPolicy *cloudPcProvisioningPolicy = [[MSGraphCloudPcProvisioningPolicy alloc] init];
[cloudPcProvisioningPolicy setDescription:@"Description value"];
[cloudPcProvisioningPolicy setDisplayName:@"Display Name value"];
MSGraphCloudPcDomainJoinConfiguration *domainJoinConfiguration = [[MSGraphCloudPcDomainJoinConfiguration alloc] init];
[domainJoinConfiguration setDomainJoinType:@"hybridAzureADJoin"];
[domainJoinConfiguration setOnPremisesConnectionId:@"16ee6c71-fc10-438b-88ac-daa1ccafffff"];
[cloudPcProvisioningPolicy setDomainJoinConfiguration:domainJoinConfiguration];
[cloudPcProvisioningPolicy setId:@"1d164206-bf41-4fd2-8424-a3192d39ffff"];
[cloudPcProvisioningPolicy setImageDisplayName:@"Windows-10 19h1-evd"];
[cloudPcProvisioningPolicy setImageId:@"MicrosoftWindowsDesktop_Windows-10_19h1-evd"];
[cloudPcProvisioningPolicy setImageType: [MSGraphCloudPcProvisioningPolicyImageType gallery]];
[cloudPcProvisioningPolicy setOnPremisesConnectionId:@"4e47d0f6-6f77-44f0-8893-c0fe1701ffff"];

NSError *error;
NSData *cloudPcProvisioningPolicyData = [cloudPcProvisioningPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:cloudPcProvisioningPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```