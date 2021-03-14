---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e20ea1d2f4dd65ec4cf7489652a5fd13185ff626
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793887"
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
    .update(calendarPermission);

```