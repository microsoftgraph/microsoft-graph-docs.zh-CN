---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1de856f119ebd6a152f2874e9566c4e0f739b664
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411677"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directorySetting = {
    values: [
        {
            name: 'CustomBlockedWordsList',
            value: 'Contoso'
        }
    ]
};

await client.api('/settings/3c105fc3-2254-4861-9e2d-d59e2126f3ef')
    .version('beta')
    .update(directorySetting);

```