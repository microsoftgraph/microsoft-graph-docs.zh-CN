---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f15d231f4f8bb2cde0ac5cf071fc48e4634cc1cf
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718329"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const confirmCompromised = {
  userIds: [
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471"
  ]
};

let res = await client.api('/riskyUsers/confirmCompromised')
    .version('beta')
    .post(confirmCompromised);

```