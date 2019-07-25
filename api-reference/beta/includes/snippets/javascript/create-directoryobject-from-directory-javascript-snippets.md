---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2ddd6d5816ea931e70ea96326b7584025780f90b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706842"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb/restore')
    .version('beta')
    .post();

```