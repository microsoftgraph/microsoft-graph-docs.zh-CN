---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d75636e8edbcb47eb77daf2c7c992ff516f42240
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808073"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/planner/plans/{id}')
    .version('beta')
    .delete();

```