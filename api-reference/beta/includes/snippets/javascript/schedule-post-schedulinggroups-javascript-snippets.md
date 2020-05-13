---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43e144aced39bcc77fb43038931ee2a628ee3717
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "36636688"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schedulingGroup = {
  displayName: "Cashiers",
  isActive: true,
  userIds: [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ]
};

let res = await client.api('/teams/{teamId}/schedule/schedulingGroups')
    .version('beta')
    .post(schedulingGroup);

```