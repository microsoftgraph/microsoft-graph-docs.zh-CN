---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3a902150a96410d61e491c02cd1d16a1cf4ee08
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621527"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/activities/13881113971988980728/')
    .version('beta')
    .delete();

```