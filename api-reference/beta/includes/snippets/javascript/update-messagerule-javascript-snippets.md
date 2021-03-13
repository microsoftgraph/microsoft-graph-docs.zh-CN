---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26bafca4dc061ce20dd231d227c3f237b6fe4e3f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786322"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const messageRule = {
    displayName: 'Important from partner',
    actions: {
        markImportance: 'high'
     }
};

await client.api('/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')')
    .version('beta')
    .update(messageRule);

```