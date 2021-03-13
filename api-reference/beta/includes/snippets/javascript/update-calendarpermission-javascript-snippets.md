---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54cc6cd4b1fc5e0fdc8cac4f3c4ece9be2786f42
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788046"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendarPermission = {
  role: 'write'
};

await client.api('/users/{id}/calendar/calendarPermissions/RGVmYXVsdA==')
    .version('beta')
    .update(calendarPermission);

```