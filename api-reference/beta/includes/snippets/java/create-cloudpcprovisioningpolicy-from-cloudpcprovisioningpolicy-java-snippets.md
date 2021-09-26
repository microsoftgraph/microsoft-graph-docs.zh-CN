---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a542756094912025517a8c23d750e2cfa80b6eced3c1dee91b03fff434cf033
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105479"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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