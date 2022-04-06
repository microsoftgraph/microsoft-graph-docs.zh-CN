---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02618a58825b3edeb4de7aa5bda23f4fad06d113
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63759017"
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
MSGraphCloudPcWindowsSettings *windowsSettings = [[MSGraphCloudPcWindowsSettings alloc] init];
[windowsSettings setLanguage:@"en-US"];
[cloudPcProvisioningPolicy setWindowsSettings:windowsSettings];

NSError *error;
NSData *cloudPcProvisioningPolicyData = [cloudPcProvisioningPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:cloudPcProvisioningPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```