---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c282631f50e5ac46a84298651a0f5ba6b64c9e0
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618508"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/dataPolicyOperations/{id}')
    .version('beta')
    .get();

```