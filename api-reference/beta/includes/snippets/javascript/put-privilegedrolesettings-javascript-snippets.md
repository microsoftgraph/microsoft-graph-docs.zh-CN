---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa8c8a223afd6c1e63325504552d2b5a609488eb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787925"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const privilegedRoleSettings = {
    id: '9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3',
    elevationDuration: 'PT8H',
    notificationToUserOnElevation: false,
    ticketingInfoOnElevation: true,
    mfaOnElevation: false,
    maxElavationDuration: 'PT0S',
    minElevationDuration: 'PT0S',
    lastGlobalAdmin: false,
    isMfaOnElevationConfigurable: true,
    approvalOnElevation: false,
    approverIds: ['e2b2a2fb-13d7-495c-adc9-941fe966793f', '22770e3f-b9b4-418e-9dea-d0e3d2f275dd']
};

await client.api('/privilegedRoles/{id}/settings')
    .version('beta')
    .put(privilegedRoleSettings);

```