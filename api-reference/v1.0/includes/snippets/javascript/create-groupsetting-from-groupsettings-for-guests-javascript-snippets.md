---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dcdab790afbfb640ea1db64d1c3cc77c6cf0982c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412690"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const groupSetting = {
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