---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe6d5100e659b882986256133aedafdad8158793
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784047"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const confirmCompromised = {
  userIds: [
    '29f270bb-4d23-4f68-8a57-dc73dc0d4caf'
  ]
};

await client.api('/identityProtection/riskyUsers/confirmCompromised')
    .version('beta')
    .post(confirmCompromised);

```