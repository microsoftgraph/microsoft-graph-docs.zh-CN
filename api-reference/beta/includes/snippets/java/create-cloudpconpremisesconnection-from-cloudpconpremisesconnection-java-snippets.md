---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bca88a3ccbfd95855513a58856ad374a2eaf935e836ac4e25c761e1c128fdd5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164053"
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