---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5444b6bf58454917e84d80714421e2eea44bfedf
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708733"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const CommsOperation = {
  metadata: "metadata-value",
  clientContext: "clientContext-value"
};

let res = await client.api('/app/calls/{id}/updateMetadata')
    .version('beta')
    .post(CommsOperation);

```