---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 432484b5452ca3b6ea8ab7f64e1509e9756540c4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978269"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcOnPremisesConnection cloudPcOnPremisesConnection = new CloudPcOnPremisesConnection();
cloudPcOnPremisesConnection.displayName = "Display Name value";
cloudPcOnPremisesConnection.subscriptionId = "0ac520ee-14c0-480f-b6c9-0a90c585ffff";
cloudPcOnPremisesConnection.subscriptionName = "Subscription Name value";
cloudPcOnPremisesConnection.adDomainName = "Active Directory Domain Name value";
cloudPcOnPremisesConnection.adDomainUsername = "Active Directory Domain User Name value";
cloudPcOnPremisesConnection.organizationalUnit = "Organization Unit value";
cloudPcOnPremisesConnection.resourceGroupId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG";
cloudPcOnPremisesConnection.virtualNetworkId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet";
cloudPcOnPremisesConnection.subnetId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default";

graphClient.deviceManagement().virtualEndpoint().onPremisesConnections()
    .buildRequest()
    .post(cloudPcOnPremisesConnection);

```