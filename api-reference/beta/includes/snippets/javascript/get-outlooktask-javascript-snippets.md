---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 583ba0e197316ac669472cfb2917c502bcf57894
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614563"
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