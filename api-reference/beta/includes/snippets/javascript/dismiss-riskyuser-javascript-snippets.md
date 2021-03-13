---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3acbab296d7cb6ada4941c2dd6237ba1733317b7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807749"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const dismiss = {
  userIds: [
    '04487ee0-f4f6-4e7f-8999-facc5a30e232'
  ]
};

await client.api('/identityProtection/riskyUsers/dismiss')
    .version('beta')
    .post(dismiss);

```