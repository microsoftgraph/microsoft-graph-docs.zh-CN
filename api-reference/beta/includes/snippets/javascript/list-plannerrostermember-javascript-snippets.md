---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4bc2ecfe7cbe1e6fe4f20a63625893e83acae24
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795201"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/planner/rosters/6519868f-868f-6519-8f86-19658f861965/members')
    .version('beta')
    .get();

```