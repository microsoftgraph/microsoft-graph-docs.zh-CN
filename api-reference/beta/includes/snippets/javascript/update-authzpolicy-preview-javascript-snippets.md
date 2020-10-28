---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ea803a2d97cb6436201b45111a36fb95b239303
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/28/2020
ms.locfileid: "48783364"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
   enabledPreviewFeatures:[
      "assignGroupsToRoles"
   ]
};

let res = await client.api('/policies/authorizationPolicy/authorizationPolicy')
    .version('beta')
    .update(authorizationPolicy);

```