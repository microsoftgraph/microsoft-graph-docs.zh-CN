---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e0f63fbf600605c2a52c9b321196c27cd5e9711
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802439"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/planner/plans/{id}')
    .delete();

```