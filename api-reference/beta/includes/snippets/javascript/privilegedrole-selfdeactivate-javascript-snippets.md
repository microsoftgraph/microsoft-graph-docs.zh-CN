---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b779729db4d53f2cdc99b1f4c6a0b2b1cc81578
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616447"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoles/{id}/selfDeactivate')
    .version('beta')
    .post();

```