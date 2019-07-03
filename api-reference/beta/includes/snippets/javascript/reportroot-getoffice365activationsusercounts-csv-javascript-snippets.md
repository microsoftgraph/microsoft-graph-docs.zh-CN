---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4a4a2fa7ef1f66418d59b6314768616a56fdd8b3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463678"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365ActivationsUserCounts')
    .version('beta')
    .get();

```