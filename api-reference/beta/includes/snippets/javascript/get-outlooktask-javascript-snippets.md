---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 583ba0e197316ac669472cfb2917c502bcf57894
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728992"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/tasks/AAMkADA1MHgwAAA=')
    .version('beta')
    .header('Prefer','outlook.timezone="Pacific Standard Time"')
    .get();

```