---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cae052c91849c3c57dc7d01a5f8325f98ab1a50c
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142568"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
  @odata.type:"#microsoft.graph.aadUserConversationMember",
  roles: ["owner"]
};

let res = await client.api('/teams/{id}/channels/{id}/members/{id}')
    .version('beta')
    .update(conversationMember);

```