---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0aaae0e4b2449ce79c7f72ac4a1e7c603ddc38d1
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394654"
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

await client.api('/groupSettings/84af2ca5-c274-41bf-86e4-6e374ec4def6')
    .update(groupSetting);

```