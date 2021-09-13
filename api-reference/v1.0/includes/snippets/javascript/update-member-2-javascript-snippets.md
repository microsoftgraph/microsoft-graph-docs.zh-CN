---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ecc34b7075586e24d6a2404cc321fa26f9518e58fe53b8e7c93952873c4fcc0a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274203"
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

await client.api('/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')
    .update(conversationMember);

```