---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d0a9160bf6d278977464afb32cca2227d4824de
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936765"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/conditionalAccess/policies/{id}')
    .version('beta')
    .delete();

```