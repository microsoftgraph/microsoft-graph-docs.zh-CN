---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f66bfc5612c9ff6fc5a11d7397580f32a28ae10f0c5091493ee41da1b3a164a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278419"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/deviceManagement/virtualEndpoint/onPremisesConnections/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphCloudPcOnPremisesConnection *cloudPcOnPremisesConnection = [[MSGraphCloudPcOnPremisesConnection alloc] init];
[cloudPcOnPremisesConnection setDisplayName:@"Display Name value"];
[cloudPcOnPremisesConnection setSubscriptionId:@"0ac520ee-14c0-480f-b6c9-0a90c585ffff"];
[cloudPcOnPremisesConnection setSubscriptionName:@"Subscription Name value"];
[cloudPcOnPremisesConnection setAdDomainName:@"Active Directory Domain Name value"];
[cloudPcOnPremisesConnection setAdDomainUsername:@"Active Directory Domain User Name value"];
[cloudPcOnPremisesConnection setOrganizationalUnit:@"Organization Unit value"];
[cloudPcOnPremisesConnection setResourceGroupId:@"/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG"];
[cloudPcOnPremisesConnection setVirtualNetworkId:@"/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet"];
[cloudPcOnPremisesConnection setSubnetId:@"/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default"];

NSError *error;
NSData *cloudPcOnPremisesConnectionData = [cloudPcOnPremisesConnection getSerializedDataWithError:&error];
[urlRequest setHTTPBody:cloudPcOnPremisesConnectionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```