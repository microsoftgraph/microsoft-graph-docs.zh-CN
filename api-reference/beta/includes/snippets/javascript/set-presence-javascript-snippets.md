---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7709833962ee97e44bfee2f602d99b103f715925
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208291"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const setPresence = {
  sessionId: '22553876-f5ab-4529-bffb-cfe50aa89f87',
  availability: 'Available',
  activity: 'Available',
  expirationDuration: 'PT1H'
};

await client.api('/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/setPresence')
    .version('beta')
    .post(setPresence);

```