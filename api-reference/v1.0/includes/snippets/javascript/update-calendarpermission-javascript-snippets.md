---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d9655d92d42669d082d8f0cdb36614f4ac35181
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806546"
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
    .update(calendarPermission);

```