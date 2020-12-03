---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af669f0636edbf5ec24a04bce86d434a92ca9048
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523168"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcProvisioningPolicy cloudPcProvisioningPolicy = new CloudPcProvisioningPolicy();
cloudPcProvisioningPolicy.displayName = "Display Name value";
cloudPcProvisioningPolicy.description = "Description value";
cloudPcProvisioningPolicy.onPremisesConnectionId = "6bf90392-5fea-459a-9e9d-a2484abbffff";
cloudPcProvisioningPolicy.imageId = "Image ID value";
cloudPcProvisioningPolicy.imageDisplayName = "Image Display Name value";
cloudPcProvisioningPolicy.imageType = CloudPcProvisioningPolicyImageType.GALLERY;

graphClient.deviceManagement().virtualEndpoint().provisioningPolicies()
    .buildRequest()
    .post(cloudPcProvisioningPolicy);

```