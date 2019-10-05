---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fa2cb14a06ec3726e26b860fecd2ea9ef57522a0
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402278"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const channel = {
  displayName: "Architecture Discussion",
  description: "This channel is where we debate all future architecture plans",
  membershipType: "standard"
};

let res = await client.api('/teams/{id}/channels')
    .version('beta')
    .post(channel);

```