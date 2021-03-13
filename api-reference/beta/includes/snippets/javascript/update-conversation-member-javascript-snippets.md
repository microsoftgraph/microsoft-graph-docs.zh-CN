---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1aa3a367aa2f0363124d36551763bae7c2e63da5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778221"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
  '@odata.type':'#microsoft.graph.aadUserConversationMember',
  roles: ['owner']
};

await client.api('/teams/{id}/channels/{id}/members/{id}')
    .version('beta')
    .update(conversationMember);

```