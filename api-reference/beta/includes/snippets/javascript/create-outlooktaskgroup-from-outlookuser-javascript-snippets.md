---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fa900d290b9acc1a1c148dcc4685304edffb52c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810547"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTaskGroup = {
  name: 'Leisure tasks'
};

await client.api('/me/outlook/taskGroups')
    .version('beta')
    .post(outlookTaskGroup);

```