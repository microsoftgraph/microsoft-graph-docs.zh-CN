---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3fd312d7fb69e11e2e664037a7df63d972d21eff
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799943"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/v1.0/users/{id}'
};

await client.api('/users/{id}/manager/$ref')
    .put(directoryObject);

```