---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff8148c8334b023ac1944e1fc85a65716b5e362442e4e0e2a018611a266cd48f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277835"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conversationMember = await client.api('/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')
    .get();

```