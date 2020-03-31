---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d6c2cc9aaab1a70db876a810a79d938ce623a5c
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062477"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/conditionalAccess/policies/{id}')
    .version('beta')
    .get();

```