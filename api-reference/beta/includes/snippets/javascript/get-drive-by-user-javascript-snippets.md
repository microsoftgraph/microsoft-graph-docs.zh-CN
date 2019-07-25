---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 068f01e8378e4f63cf7325052cb271a2ce7d8c68
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706484"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{idOrUserPrincipalName}/drive')
    .version('beta')
    .get();

```