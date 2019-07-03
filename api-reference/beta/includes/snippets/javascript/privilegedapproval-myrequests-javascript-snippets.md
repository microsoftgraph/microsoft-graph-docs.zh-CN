---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4f7bf5cab65c8f55cb616cb92c8f4df25a260f7d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479223"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedApproval/myRequests')
    .version('beta')
    .get();

```