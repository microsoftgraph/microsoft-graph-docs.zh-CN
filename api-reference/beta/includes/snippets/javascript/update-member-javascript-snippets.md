---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7fa65eefd62de08be50b15b04f13820b39eafa62
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522018"
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

let res = await client.api('/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')
    .version('beta')
    .update(conversationMember);

```