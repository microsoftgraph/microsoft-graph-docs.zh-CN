---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe9e9ff4015fac8298c1de523d463f96d633b9b3
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46570144"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const dismiss = {
  userIds: [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232"
  ]
};

let res = await client.api('/identityProtection/riskyUsers/dismiss')
    .version('beta')
    .post(dismiss);

```