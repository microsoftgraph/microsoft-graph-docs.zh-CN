---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43e144aced39bcc77fb43038931ee2a628ee3717
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
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