---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a0fa29090b841f5f54299424e16c813dc6ea233
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513040"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const groupSetting = {
  displayName: 'Group.Unified.Guest',
  templateId: '08d542b9-071f-4e16-94b0-74abb372e3d9',
  values: [
    {
      name: 'AllowToAddGuests',
      value: 'false'
    }
  ]
};

await client.api('/groups/055a5d18-a3a9-4338-b9c5-de92559b7ebf/settings')
    .post(groupSetting);

```