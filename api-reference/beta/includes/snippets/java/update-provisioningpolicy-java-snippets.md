---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23cd814e03151d45dbfd1ef851e8113274de3ef3
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758875"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcProvisioningPolicy cloudPcProvisioningPolicy = new CloudPcProvisioningPolicy();
cloudPcProvisioningPolicy.displayName = "HR provisioning policy";
cloudPcProvisioningPolicy.description = "Provisioning policy for India HR employees";
cloudPcProvisioningPolicy.onPremisesConnectionId = "4e47d0f6-6f77-44f0-8893-c0fe1701ffff";
cloudPcProvisioningPolicy.imageId = "Image ID value";
cloudPcProvisioningPolicy.imageDisplayName = "Image Display Name value";
cloudPcProvisioningPolicy.imageType = CloudPcProvisioningPolicyImageType.CUSTOM;
CloudPcWindowsSettings windowsSettings = new CloudPcWindowsSettings();
windowsSettings.language = "en-US";
cloudPcProvisioningPolicy.windowsSettings = windowsSettings;

graphClient.deviceManagement().virtualEndpoint().provisioningPolicies("{id}")
    .buildRequest()
    .patch(cloudPcProvisioningPolicy);

```