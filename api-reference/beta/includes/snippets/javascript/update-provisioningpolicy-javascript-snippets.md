---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4cab25e9afb0b6f740f9116b11874f12c4841080fda75b5ccff6873b1294dec3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278415"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cloudPcProvisioningPolicy = {
  '@odata.type': '#microsoft.graph.cloudPcProvisioningPolicy',
  displayName: 'Display Name value',
  description: 'Description value',
  onPremisesConnectionId: '4e47d0f6-6f77-44f0-8893-c0fe1701ffff',
  imageId: 'Image ID value',
  imageDisplayName: 'Image Display Name value',
  imageType: 'custom'
};

await client.api('/deviceManagement/virtualEndpoint/provisioningPolicies/{id}')
    .version('beta')
    .update(cloudPcProvisioningPolicy);

```