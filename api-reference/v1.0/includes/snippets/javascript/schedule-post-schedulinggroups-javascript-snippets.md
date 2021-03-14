---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ca451c9e3262d4e2fe8069eba21aaec77c7e8cf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779653"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schedulingGroup = {
  displayName: 'Cashiers',
  isActive: true,
  userIds: [
    'c5d0c76b-80c4-481c-be50-923cd8d680a1',
    '2a4296b3-a28a-44ba-bc66-0274b9b95851'
  ]
};

await client.api('/teams/{teamId}/schedule/schedulingGroups')
    .post(schedulingGroup);

```