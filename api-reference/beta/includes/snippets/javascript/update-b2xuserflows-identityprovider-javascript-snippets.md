---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2c4c157e75484d17fbef80daa26f59cfe6d9861
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785506"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProviders = {
  '@odata.id': 'https://graph.microsoft.com/beta/identityProviders/{id}'
};

await client.api('/identity/b2xUserFlows/{id}/identityProviders/$ref')
    .version('beta')
    .update(identityProviders);

```