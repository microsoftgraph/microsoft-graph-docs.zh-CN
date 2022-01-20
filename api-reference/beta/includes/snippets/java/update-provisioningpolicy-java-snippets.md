---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68b466fedaadd84833f77c00b7e269232e2b4282
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131444"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcProvisioningPolicy cloudPcProvisioningPolicy = new CloudPcProvisioningPolicy();
cloudPcProvisioningPolicy.displayName = "HR provisioning policy";
cloudPcProvisioningPolicy.description = "Provisioning policy for India HR employees";
cloudPcProvisioningPolicy.onPremisesConnectionId = "4e47d0f6-6f77-44f0-8893-c0fe1701b553";

graphClient.deviceManagement().virtualEndpoint().provisioningPolicies("{id}")
    .buildRequest()
    .patch(cloudPcProvisioningPolicy);

```