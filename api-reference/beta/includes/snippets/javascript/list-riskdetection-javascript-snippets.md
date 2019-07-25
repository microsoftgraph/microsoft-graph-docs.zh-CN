---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3d0be37be4e95d7bb4a484d87e8b79ac91428a56
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725755"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/riskDetections')
    .version('beta')
    .get();

```