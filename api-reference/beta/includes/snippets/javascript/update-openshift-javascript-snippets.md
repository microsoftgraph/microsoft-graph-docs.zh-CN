---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8e6eab6d9853e3bb930701c28dbae4a08ce833a
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44219218"
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

let res = await client.api('/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8')
    .version('beta')
    .put(openShift);

```