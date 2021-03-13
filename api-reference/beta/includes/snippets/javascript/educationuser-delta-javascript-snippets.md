---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 247789ecb539c3469f81bba00234b73e22a3b6d2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804686"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/education/users/delta')
    .version('beta')
    .get();

```