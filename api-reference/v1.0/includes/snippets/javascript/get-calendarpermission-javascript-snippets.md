---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dacaa82e4361fc9e3cf9cf405e8251b98c6eeb70
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806579"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/calendar/calendarPermissions/{id}')
    .get();

```