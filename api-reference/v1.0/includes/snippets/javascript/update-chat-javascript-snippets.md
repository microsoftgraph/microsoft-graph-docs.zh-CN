---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ddb5d7af0972cd634516238805465ed944cd8a0a2ce155ac140dbcf248b24dd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106813"
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
    .update(chat);

```