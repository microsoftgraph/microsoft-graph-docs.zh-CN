---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 900a908fb88a3f029fd2b07d0301c1bfa78f0282
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782647"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviders = await client.api('/identity/b2xUserFlows/{id}/identityProviders')
    .version('beta')
    .get();

```