---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74871f744396f812177e82e62d2e421533d059f4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799272"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let my = await client.api('/privilegedRoleAssignments/my')
    .version('beta')
    .get();

```