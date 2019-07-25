---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 002e323890cbd2bef7e8c5ee76823d563877e3f8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708811"
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