---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea4b945d8713bc5187211e7aafbd4f59efd9980c
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992433"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schedule = {
   enabled: true,
   timeZone: 'America/Chicago',
   provisionStatus: 'Completed',
   provisionStatusCode: null,
   openShiftsEnabled: true,
   swapShiftsRequestsEnabled: true,
   offerShiftRequestsEnabled: true,
   timeOffRequestsEnabled: true,
   timeClockEnabled: true,
   timeClockSettings: {
      approvedLocation: {
         altitude: 1024.13,
         latitude: 26.13246,
         longitude: 24.34616
      }
   }
};

await client.api('/teams/871dbd5c-3a6a-4392-bfe1-042452793a50/schedule')
    .version('beta')
    .put(schedule);

```