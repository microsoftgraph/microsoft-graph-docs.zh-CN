---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a726124b7f68d42ddf32f3cee4823f95fdb326bc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803094"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
'@odata.id': 'https://graph.microsoft.com/beta/directoryObjects/{id}'
};

await client.api('/applications/{id}/owners/$ref')
    .version('beta')
    .post(directoryObject);

```