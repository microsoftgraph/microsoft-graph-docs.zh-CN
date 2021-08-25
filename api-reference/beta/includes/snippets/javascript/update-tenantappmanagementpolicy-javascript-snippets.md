---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4936cb4184466537dfda79de84f9617c1ad4e354
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513821"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tenantAppManagementPolicy = {
    isEnabled: true,
    applicationRestrictions: {
        passwordCredentials: [
            {
                restrictionType: 'passwordAddition',
                maxLifetime: null,
                restrictForAppsCreatedAfterDateTime: '2021-04-01T10:37:00Z'
            },
            {
                restrictionType: 'passwordLifetime',
                maxLifetime: 'P4DT12H30M5S',
                restrictForAppsCreatedAfterDateTime: '2019-01-01T10:37:00Z'
            }
        ]
    }
};

await client.api('/policies/defaultAppManagementPolicy')
    .version('beta')
    .update(tenantAppManagementPolicy);

```