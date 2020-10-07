---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f72dc5b1515bdba129d20ab7ca50a601c1e778b
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "48373290"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const servicePrincipal = {
  appId:"d7fbfe28-c60e-46d2-8335-841923950d3b",
  tags: [
    "WindowsAzureActiveDirectoryIntegratedApp",
    "WindowsAzureActiveDirectoryOnPremApp"
  ]
};

let res = await client.api('/serviceprincipals')
    .version('beta')
    .post(servicePrincipal);

```