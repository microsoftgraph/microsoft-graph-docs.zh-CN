---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e40d5bc6ea8a495fa902cc8d3c66a3ca0d87e050
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48622533"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/AAMkAGVmMDEzN')
    .version('beta')
    .get();

```