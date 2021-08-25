---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ede11a88b8fe8515c347b30d75831f50f94cbf97
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514621"
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
      value: 'false'
    }
  ]
};

await client.api('/groupSettings/f0b2d6f5-097d-4177-91af-a24e530b53cc')
    .update(groupSetting);

```