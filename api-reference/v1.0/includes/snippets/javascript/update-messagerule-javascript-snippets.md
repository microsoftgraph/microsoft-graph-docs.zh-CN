---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f34ed2f24804f525e3d19cda274325b09160ad17
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800022"
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

await client.api('/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=')
    .update(messageRule);

```