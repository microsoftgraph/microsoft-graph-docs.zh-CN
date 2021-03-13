---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b4a9863fde051581d65126d1a340a8386dc9d31
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808606"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chat = {
    topic: 'Group chat title update'
};

await client.api('/chats/19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2')
    .version('beta')
    .update(chat);

```