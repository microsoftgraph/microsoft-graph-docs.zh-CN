---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c650536e2245aa865ad5656dc4a1619e7449e66
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776177"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appRoleAssignments = await client.api('/users/cdb555e3-b33e-4fd5-a427-17fadacbdfa7/appRoleAssignments')
    .version('beta')
    .get();

```