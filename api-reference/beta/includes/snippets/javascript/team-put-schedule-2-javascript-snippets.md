---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b200c384987b585cb9b637372b7a458f1f697f53edd1d11682c6c2a552aab541
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103933"
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