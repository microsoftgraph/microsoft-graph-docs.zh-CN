---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a70af8a8745ff19f91122772b245293e07f1281e
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52871515"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conversationMember = await client.api('/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')
    .get();

```