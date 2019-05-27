---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d5a35212935d014cf66ca478ca89a9d2f6bbd4f0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34455479"
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