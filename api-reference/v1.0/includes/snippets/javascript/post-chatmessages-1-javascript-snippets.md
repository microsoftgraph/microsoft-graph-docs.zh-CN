---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80be1127c104eff6b4035a0740b44eb6fb872d3cf4ed4e196dce2b7c8aabac21
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328900"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
  body: {
     content: 'Hello world'
  }
};

await client.api('/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages')
    .post(chatMessage);

```