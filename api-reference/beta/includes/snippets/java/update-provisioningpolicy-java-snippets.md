---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bb1507718fce5e448d6e3578a19e5231529c686739bc6ae06d28ea2fce8f999
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278416"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcProvisioningPolicy cloudPcProvisioningPolicy = new CloudPcProvisioningPolicy();
cloudPcProvisioningPolicy.displayName = "Display Name value";
cloudPcProvisioningPolicy.description = "Description value";
cloudPcProvisioningPolicy.onPremisesConnectionId = "4e47d0f6-6f77-44f0-8893-c0fe1701ffff";
cloudPcProvisioningPolicy.imageId = "Image ID value";
cloudPcProvisioningPolicy.imageDisplayName = "Image Display Name value";
cloudPcProvisioningPolicy.imageType = CloudPcProvisioningPolicyImageType.CUSTOM;

graphClient.deviceManagement().virtualEndpoint().provisioningPolicies("{id}")
    .buildRequest()
    .patch(cloudPcProvisioningPolicy);

```