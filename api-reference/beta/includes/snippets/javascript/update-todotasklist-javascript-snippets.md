---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6dfc22cc7a34d2b407011c9173ced12c3d12fd4
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873118"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const aAMkADIyAAAhrbPWAAA= = {
  displayName: "Vacation Plan",
};

let res = await client.api('/me/todo/lists/AAMkADIyAAAhrbPWAAA=')
    .version('beta')
    .update(aAMkADIyAAAhrbPWAAA=);

```