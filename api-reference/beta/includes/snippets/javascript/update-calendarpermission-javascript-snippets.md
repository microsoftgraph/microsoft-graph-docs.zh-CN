---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ae9e43ccce07abc1773a5db781eb3ebb11089ac
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41778024"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendarPermission = {
  role: "write"
};

let res = await client.api('/users/{id}/calendar/calendarPermissions/RGVmYXVsdA==')
    .version('beta')
    .update(calendarPermission);

```