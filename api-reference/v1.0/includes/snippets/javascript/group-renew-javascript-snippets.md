---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e22c4464c2f52d18f437b1b9f7c775fd9aad1c7
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616186"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/renew')
    .post();

```