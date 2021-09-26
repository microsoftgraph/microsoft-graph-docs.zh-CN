---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5ccd0781d0de53e79b21aa7fa129ab1aa016bf3ce8c276b87c2938cfc002082
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220833"
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

graphClient.deviceManagement().virtualEndpoint().onPremisesConnections("{id}")
    .buildRequest()
    .patch(cloudPcOnPremisesConnection);

```