---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0988955da910fafaab5c5c18af966860c520cc9592cb7a59096375d9795206ed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220613"
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