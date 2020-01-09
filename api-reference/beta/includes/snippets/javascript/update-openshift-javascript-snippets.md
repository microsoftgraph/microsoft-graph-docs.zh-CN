---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fee56dc24fc193987e4b13622c2539c62ce846e2
ms.sourcegitcommit: 66c8fcafee151278f8089cd26d0c5766d33d04a8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/09/2020
ms.locfileid: "40995364"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const openShift = {
schedulingGroupId: "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
sharedOpenShift: {
notes: "Inventory Management",
openSlotCount:5,
displayName: "Field shift",
startDateTime: "2018-10-04T00:58:45.340Z",
endDateTime: "2018-10-04T09:50:45.332Z",
theme: "white",
activities: [
{
isPaid: true,
startDateTime: "2018-10-04T00:58:45.340Z",
endDateTime: "2018-10-04T01:58:45.340Z",
code: "",
displayName: "Lunch"
}
]
},
draftOpenShift: null
};

let res = await client.api('/teams/{id}/schedule/openShifts/{openShiftId}')
    .version('beta')
    .put(openShift);

```