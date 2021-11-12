---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3071a652c21de0d81f803c7bb93d6c7019f7ec773a3e88f7362501ae06581bb0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220076"
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
    .version('beta')
    .post(schedulingGroup);

```