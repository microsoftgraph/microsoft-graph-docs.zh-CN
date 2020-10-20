---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5636d2cd92bb4c0ca47707980ac348e3d8932f82
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618528"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles/delta')
    .version('beta')
    .get();

```