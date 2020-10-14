---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6080a0779a861dda11f24d72aa248aac8340da98
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458870"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/authentication/fido2Methods')
    .version('beta')
    .get();

```