---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 66e2f2b0c9b6af9af08eaa4a239077ad9a62dfde
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633909"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
  @odata.type: "microsoft.graph.aadConversationMember",
  roles: [],
  user@odata.bind: "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
};

let res = await client.api('/teams/{id}/channels/{id}/members/')
    .version('beta')
    .post(conversationMember);

```