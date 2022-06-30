---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ace158d4445825b5ef871d0bdce68f0449fc3de
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440575"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcProvisioningPolicy = await client.api('/deviceManagement/virtualEndpoint/provisioningPolicies/60b94f83-3e22-430e-a69d-440f65b922d6')
    .version('beta')
    .select('id,description,displayName,domainJoinConfiguration,imageDisplayName,imageId,imageType,onPremisesConnectionId,windowsSettings,managedBy,cloudPcGroupDisplayName,gracePeriodInHours,localAdminEnabled,alternateResourceUrl')
    .get();

```