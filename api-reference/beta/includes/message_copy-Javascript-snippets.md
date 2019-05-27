---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bed22468e6ad7a2d56814394b65c1a01a135aa5d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444151"
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
    .version('beta')
    .post(message);

```