---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d518da946d886ac8b46480fd68a1de6068ddc7cd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810223"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schedule = {
  enabled: true,
  timeZone: 'America/Chicago'
};

await client.api('/teams/{teamId}/schedule')
    .version('beta')
    .put(schedule);

```