---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2dc230a100ab8f80ce0a7a8afcda52601abd2457
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783568"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const groupSetting = {
  displayName: 'GroupSettings',
  templateId: '08d542b9-071f-4e16-94b0-74abb372e3d9',
  values: [
    {
            name: 'AllowToAddGuests',
            value: 'false'
    }
  ]
};

await client.api('/groups/{id}/settings/{id}')
    .update(groupSetting);

```