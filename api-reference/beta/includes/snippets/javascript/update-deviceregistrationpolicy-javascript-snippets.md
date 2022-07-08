---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c837a960a118fd67f5dabad5cc51e70f1b71f77c
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65695226"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const deviceRegistrationPolicy = {
    id: 'deviceRegistrationPolicy',
    displayName: 'Device Registration Policy',
    description: 'Tenant-wide policy that manages intial provisioning controls using quota restrictions, additional authentication and authorization checks',
    userDeviceQuota: 50,
    multiFactorAuthConfiguration: '0',
    azureADRegistration: {
        appliesTo: '1',
        isAdminConfigurable: false,
        allowedUsers: [],
        allowedGroups: []
    },
    azureADJoin: {
        appliesTo: '1',
        isAdminConfigurable: true,
        allowedUsers: [],
        allowedGroups: []
    }
};

await client.api('/deviceRegistrationPolicy')
    .version('beta')
    .put(deviceRegistrationPolicy);

```