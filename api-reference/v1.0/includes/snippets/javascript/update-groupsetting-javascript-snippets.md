---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24b9581a911301bdba11931360bb350a685b2b29
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947078"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const groupSetting = {
  displayName: "GroupSettings",
  templateId: "08d542b9-071f-4e16-94b0-74abb372e3d9",
  values: [
    {
            name: "AllowToAddGuests",
            value: "false"
    }
  ]
};

let res = await client.api('/groups/{id}/settings/{id}')
    .update(groupSetting);

```