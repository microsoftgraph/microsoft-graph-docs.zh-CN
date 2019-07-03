---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d888b3e604a5866af3029e5319b9dea1b53624b9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520422"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/applicationSignInDetailedSummary/'id'')
    .version('beta')
    .get();

```