---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3d6f44d66efc89fce84fa7177832aeaf1a8cc00
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798570"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  '@odata.id':'https://graph.microsoft.com/beta/education/users/14008'
};

await client.api('/education/schools/{id}/users/$ref')
    .version('beta')
    .post(educationUser);

```