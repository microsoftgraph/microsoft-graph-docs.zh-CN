---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ebd7e1cb32aacb510d2a07f38aed4ceddef7159
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959932"
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