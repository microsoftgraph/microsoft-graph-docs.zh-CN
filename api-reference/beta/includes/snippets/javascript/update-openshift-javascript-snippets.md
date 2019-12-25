---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ea710aa83f947eab040be74a4bfe7245e4974cd
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867789"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const openShifts = {
  sharedOpenShift: {
    openSlotCount: 99
  },
  draftOpenShift: {
    openSlotCount: 99
  },
  schedulingGroupId: "TAG_f914d037-00a3-4ba4-b712-ef178cbea263"
};

let res = await client.api('/teams/{id}/schedule/openShifts')
    .version('beta')
    .update(openShifts);

```