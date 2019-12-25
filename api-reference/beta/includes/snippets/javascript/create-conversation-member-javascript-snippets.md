---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39a257f6fc52f94d16611e77f84e3cc0bdf18f11
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868739"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
  @odata.type: "#microsoft.graph.aadUserConversationMember",
  roles: [],
  user@odata.bind: "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
};

let res = await client.api('/teams/{id}/channels/{id}/members/')
    .version('beta')
    .post(conversationMember);

```