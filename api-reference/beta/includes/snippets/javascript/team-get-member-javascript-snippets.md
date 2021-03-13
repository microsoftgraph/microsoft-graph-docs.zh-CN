---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7cbf55351a1e8a7e2ccb837f17ec131b5232e59
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808513"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conversationMember = await client.api('/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/members//ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')
    .version('beta')
    .get();

```