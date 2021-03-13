---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8aa74ef6ba7868273e0e76f7428d667861dc77a3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771440"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  '@odata.id': 'https://graph.microsoft.com/v1.0/users/{userId}'
};

await client.api('/print/shares/{printerShareId}/allowedUsers/$ref')
    .post(user);

```