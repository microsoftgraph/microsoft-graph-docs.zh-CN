---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57a32106b83572c7eade78f8597180bd405dd503
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890220"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id':'https://graph.microsoft.com/beta/groups/{id}'
};

await client.api('/administrativeUnits/{id}/members/$ref')
    .version('beta')
    .post(directoryObject);

```