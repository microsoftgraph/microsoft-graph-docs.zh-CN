---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: baed0ee22c3abee6f648f62fe0e1e86143a3d628
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780018"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const presence = {
  ids: ['fa8bf3dc-eca7-46b7-bad1-db199b62afc3', '66825e03-7ef5-42da-9069-724602c31f6b']
};

await client.api('/communications/getPresencesByUserId')
    .version('beta')
    .post(presence);

```