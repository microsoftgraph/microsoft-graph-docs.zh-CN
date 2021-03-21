---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4caa689114fa1e3adad32de33c7e8a5727d5602
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960833"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const dismiss = {
  userIds: [
    '04487ee0-f4f6-4e7f-8999-facc5a30e232',
    '13387ee0-f4f6-4e7f-8999-facc5120e345'
  ]
};

await client.api('/riskyUsers/dismiss')
    .version('beta')
    .post(dismiss);

```