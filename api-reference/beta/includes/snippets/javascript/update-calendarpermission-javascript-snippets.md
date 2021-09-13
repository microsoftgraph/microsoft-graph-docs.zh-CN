---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b61f56936a7936c2ec05f96ec094695cd6957a90037bb53bae80a0d2f7d5b44
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163447"
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