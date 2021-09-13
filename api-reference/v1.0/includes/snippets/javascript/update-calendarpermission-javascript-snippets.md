---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6612bf558e30b3a1b36fc445e45d2414d18b07596734f3b5284dc368caa12053
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219893"
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