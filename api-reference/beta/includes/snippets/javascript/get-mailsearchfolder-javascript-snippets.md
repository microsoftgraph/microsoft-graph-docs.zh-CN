---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e40d5bc6ea8a495fa902cc8d3c66a3ca0d87e050
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721694"
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