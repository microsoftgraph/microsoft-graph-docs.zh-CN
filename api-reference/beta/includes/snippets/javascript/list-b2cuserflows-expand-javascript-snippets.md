---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1277b386ffa27dc9ff54f48638bd9e3798ca3931
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329818"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/b2cUserFlows')
    .version('beta')
    .expand('identityProviders')
    .get();

```