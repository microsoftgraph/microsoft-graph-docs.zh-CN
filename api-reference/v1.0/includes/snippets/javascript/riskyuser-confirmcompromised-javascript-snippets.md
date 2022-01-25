---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37a918498ed025981b04e26b2af77a5e8ec4ec50
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088194"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const confirmCompromised = {
  userIds: [
    '29f270bb-4d23-4f68-8a57-dc73dc0d4caf',
    '20f91ec9-d140-4d90-9cd9-f618587a1471'
  ]
};

await client.api('/identityProtection/riskyUsers/confirmCompromised')
    .post(confirmCompromised);

```