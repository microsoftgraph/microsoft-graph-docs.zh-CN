---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4f7bf5cab65c8f55cb616cb92c8f4df25a260f7d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728593"
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