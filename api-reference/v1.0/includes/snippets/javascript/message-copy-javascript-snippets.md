---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d5a35212935d014cf66ca478ca89a9d2f6bbd4f0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732233"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  destinationId: "destinationId-value"
};

let res = await client.api('/me/messages/{id}/copy')
    .post(message);

```