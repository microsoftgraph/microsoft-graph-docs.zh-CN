---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b3826496e0e4eea9f6bdf99ce60c7df9ff9b6a3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786364"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendarPermission = await client.api('/users/{id}/calendar/calendarPermissions/{id}')
    .version('beta')
    .get();

```