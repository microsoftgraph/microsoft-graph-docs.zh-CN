---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45ffcf96a86af2def026d03a2855afa7c961be2f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37994864"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/calendar/calendarPermissions/{id}')
    .version('beta')
    .get();

```