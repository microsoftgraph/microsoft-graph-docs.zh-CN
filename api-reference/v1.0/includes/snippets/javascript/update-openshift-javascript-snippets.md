---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ee5409776d3b0ee0479255915601b2e0e5171fd8ea8b1e25ad9aa2dbc776ac1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218731"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const openShift = {
schedulingGroupId: 'TAG_228940ed-ff84-4e25-b129-1b395cf78be0',
sharedOpenShift: {
notes: 'Inventory Management',
openSlotCount: 5,
displayName: 'Field shift',
startDateTime: '2018-10-04T00:58:45.340Z',
endDateTime: '2018-10-04T09:50:45.332Z',
theme: 'white',
activities: [
{
isPaid: true,
startDateTime: '2018-10-04T00:58:45.340Z',
endDateTime: '2018-10-04T01:58:45.340Z',
code: '',
displayName: 'Lunch'
}
]
},
draftOpenShift: null
};

await client.api('/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8')
    .update(openShift);

```