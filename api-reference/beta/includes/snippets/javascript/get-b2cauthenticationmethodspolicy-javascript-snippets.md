---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6014d967291260a40bbbece4a0e3e8130b98a0a
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457340"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/b2cAuthenticationMethodsPolicy')
    .version('beta')
    .get();

```