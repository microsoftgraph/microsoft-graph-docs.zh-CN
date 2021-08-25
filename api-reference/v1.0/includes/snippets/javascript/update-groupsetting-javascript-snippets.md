---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e40aba07b1acc22b1554f25b7c2d546ea0b554e5
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514618"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const groupSetting = {
  values: [
    {
      name: 'AllowToAddGuests',
      value: 'true'
    }
  ]
};

await client.api('/groups/0167b5af-f3d1-4910-82d2-398747fa381c/settings/fa6df613-159b-4f94-add2-7093f961900b')
    .update(groupSetting);

```