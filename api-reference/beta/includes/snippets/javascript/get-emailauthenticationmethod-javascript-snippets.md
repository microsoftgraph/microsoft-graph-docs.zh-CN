---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5fb88bef20e4fc4d241e03c93ab668e721ff4fcc
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458155"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/authentication/emailMethods')
    .version('beta')
    .get();

```