---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f194617c48ed1a27da6bc55800838906381b8d45
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786851"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id':'https://graph.microsoft.com/beta/users/alexd@contoso.com'
};

await client.api('/groups/{id}/rejectedSenders/$ref')
    .version('beta')
    .post(directoryObject);

```