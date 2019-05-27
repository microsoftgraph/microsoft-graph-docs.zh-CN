---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 002e323890cbd2bef7e8c5ee76823d563877e3f8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456184"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const CommsOperation = {
  clientContext: "d45324c1-fcb5-430a-902c-f20af696537c"
};

let res = await client.api('/app/calls/{id}/subscribeToTone')
    .version('beta')
    .post(CommsOperation);

```