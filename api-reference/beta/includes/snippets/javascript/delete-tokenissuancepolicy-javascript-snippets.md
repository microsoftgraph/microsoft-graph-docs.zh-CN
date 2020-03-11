---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 261ae1f691f106d25297822cd771c22dd7b35f74
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591759"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/tokenIssuancePolicies/{id}')
    .version('beta')
    .delete();

```