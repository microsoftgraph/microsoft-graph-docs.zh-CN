---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f1636850e2a3fada1908aa414438ac9bc44124df3d9227b2522718027646c4b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105476"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/deviceManagement/virtualEndpoint/provisioningPolicies"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphCloudPcProvisioningPolicy *cloudPcProvisioningPolicy = [[MSGraphCloudPcProvisioningPolicy alloc] init];
[cloudPcProvisioningPolicy setDisplayName:@"Display Name value"];
[cloudPcProvisioningPolicy setDescription:@"Description value"];
[cloudPcProvisioningPolicy setOnPremisesConnectionId:@"6bf90392-5fea-459a-9e9d-a2484abbffff"];
[cloudPcProvisioningPolicy setImageId:@"Image ID value"];
[cloudPcProvisioningPolicy setImageDisplayName:@"Image Display Name value"];
[cloudPcProvisioningPolicy setImageType: [MSGraphCloudPcProvisioningPolicyImageType gallery]];

NSError *error;
NSData *cloudPcProvisioningPolicyData = [cloudPcProvisioningPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:cloudPcProvisioningPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```