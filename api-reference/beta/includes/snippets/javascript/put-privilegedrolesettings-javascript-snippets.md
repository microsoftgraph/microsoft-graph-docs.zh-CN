---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 62366f49f3da3db025a2c7bb676fc68fa734e4b0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500300"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const privilegedRoleSettings = {
    id: "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
    elevationDuration: "PT8H",
    notificationToUserOnElevation: false,
    ticketingInfoOnElevation: true,
    mfaOnElevation: false,
    maxElavationDuration: "PT0S",
    minElevationDuration: "PT0S",
    lastGlobalAdmin: false,
    isMfaOnElevationConfigurable: true,
    approvalOnElevation: false,
    approverIds: ["e2b2a2fb-13d7-495c-adc9-941fe966793f", "22770e3f-b9b4-418e-9dea-d0e3d2f275dd"]
};

let res = await client.api('/privilegedRoles/{id}/settings')
    .version('beta')
    .put({privilegedRoleSettings : privilegedRoleSettings});

```