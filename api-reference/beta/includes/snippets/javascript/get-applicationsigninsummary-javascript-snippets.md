---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 34ae62364bb5aac81c99edbff8bd0b7fd5d72787
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479497"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getAzureADApplicationSignInSummary(period='D7')')
    .version('beta')
    .get();

```