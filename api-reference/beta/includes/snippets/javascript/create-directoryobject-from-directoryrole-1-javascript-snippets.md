---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d0429d61ea92c0be1328010e36662f1f58e836d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946577"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
    '@odata.id':'https://graph.microsoft.com/beta/users/0f933635-5b77-4cf4-a577-f78a5eb090a2'
};

await client.api('/directoryRoles/0afed502-2456-4fd4-988e-3c21924c28a7/members/$ref')
    .version('beta')
    .post(directoryObject);

```