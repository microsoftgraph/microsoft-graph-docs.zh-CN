---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5b5d5d6b84e1c8d6bc1c9f6621388cf2b741033
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349840"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcOnPremisesConnection cloudPcOnPremisesConnection = new CloudPcOnPremisesConnection();
cloudPcOnPremisesConnection.displayName = "test-canary-02";
cloudPcOnPremisesConnection.type = CloudPcOnPremisesConnectionType.HYBRID_AZURE_A_D_JOIN;
cloudPcOnPremisesConnection.subscriptionId = "0ac520ee-14c0-480f-b6c9-0a90c585ffff";
cloudPcOnPremisesConnection.subscriptionName = "CPC customer 001 test subscription";
cloudPcOnPremisesConnection.adDomainName = "contoso001.com";
cloudPcOnPremisesConnection.adDomainUsername = "dcadmin";
cloudPcOnPremisesConnection.organizationalUnit = "OU=Domain Controllers, DC=contoso001, DC=com";
cloudPcOnPremisesConnection.resourceGroupId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG";
cloudPcOnPremisesConnection.virtualNetworkId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET";
cloudPcOnPremisesConnection.subnetId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET/subnets/canary01-Subnet";

graphClient.deviceManagement().virtualEndpoint().onPremisesConnections()
    .buildRequest()
    .post(cloudPcOnPremisesConnection);

```