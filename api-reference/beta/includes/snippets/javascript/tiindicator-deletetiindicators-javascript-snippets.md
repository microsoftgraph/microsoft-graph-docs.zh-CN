---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f69cfc9636fe5e6c977b293576501aacf7f2ee07
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479312"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const ResultInfo = {
  value: [
    "id-value1",
    "id-value2"
  ]
};

let res = await client.api('/security/tiIndicators/deleteTiIndicators')
    .version('beta')
    .post(ResultInfo);

```