---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4bbcf6ac726ba28a4abb317e44d5da213961673d
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329496"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProviders = {
  @odata.id: "https://graph.microsoft.com/beta/identityProviders/{id}"
};

let res = await client.api('/identity/b2xUserFlows/{id}/identityProviders/$ref')
    .version('beta')
    .update(identityProviders);

```