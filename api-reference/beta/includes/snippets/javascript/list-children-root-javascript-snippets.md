---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c37218459ae43302ae2b2462031317843d278bb
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613200"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/children')
    .version('beta')
    .get();

```