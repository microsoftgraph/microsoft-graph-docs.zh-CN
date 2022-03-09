---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8f1057344244d684dc152bcb4f2b84f150f8fe4
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395767"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directorySetting = {
    templateId: '08d542b9-071f-4e16-94b0-74abb372e3d9',
    values: [
        {
            name: 'AllowToAddGuests',
            value: 'false'
        }
    ]
};

await client.api('/groups/05aa6a98-956a-45c0-b13b-88076a23f2cd/settings')
    .version('beta')
    .post(directorySetting);

```