---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ebd7e1cb32aacb510d2a07f38aed4ceddef7159
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808847"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/v1.0/directoryObjects/{id}'
};

await client.api('/devices/{id}/registeredOwners/$ref')
    .post(directoryObject);

```