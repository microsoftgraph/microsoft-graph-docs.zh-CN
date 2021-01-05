---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7eb12fcee43bfff58fd07fe1788baaae31f946bb
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753917"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chat = {
    topic: "Group chat title update",
};

let res = await client.api('/chats/19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2')
    .version('beta')
    .update(chat);

```