---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8746a9a2cf6e6466c871f4eae124749cbd6d171
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349630"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/deviceManagement/virtualEndpoint/onPremisesConnections"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphCloudPcOnPremisesConnection *cloudPcOnPremisesConnection = [[MSGraphCloudPcOnPremisesConnection alloc] init];
[cloudPcOnPremisesConnection setDisplayName:@"test-canary-02"];
[cloudPcOnPremisesConnection setType: [MSGraphCloudPcOnPremisesConnectionType hybridAzureADJoin]];
[cloudPcOnPremisesConnection setSubscriptionId:@"0ac520ee-14c0-480f-b6c9-0a90c585ffff"];
[cloudPcOnPremisesConnection setSubscriptionName:@"CPC customer 001 test subscription"];
[cloudPcOnPremisesConnection setAdDomainName:@"contoso001.com"];
[cloudPcOnPremisesConnection setAdDomainUsername:@"dcadmin"];
[cloudPcOnPremisesConnection setOrganizationalUnit:@"OU=Domain Controllers, DC=contoso001, DC=com"];
[cloudPcOnPremisesConnection setResourceGroupId:@"/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG"];
[cloudPcOnPremisesConnection setVirtualNetworkId:@"/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET"];
[cloudPcOnPremisesConnection setSubnetId:@"/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET/subnets/canary01-Subnet"];

NSError *error;
NSData *cloudPcOnPremisesConnectionData = [cloudPcOnPremisesConnection getSerializedDataWithError:&error];
[urlRequest setHTTPBody:cloudPcOnPremisesConnectionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```