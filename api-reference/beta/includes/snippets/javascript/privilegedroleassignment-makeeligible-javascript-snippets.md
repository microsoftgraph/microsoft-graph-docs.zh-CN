---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f843743b0915ba7cb0d716592396508785f770d3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781864"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/privilegedRoleAssignments/{id}/makeEligible')
    .version('beta')
    .post();

```