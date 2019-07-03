---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 66afc96e5c0004eae253bd06c95e8bdd7a3bd5f7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520125"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  @odata.type: "microsoft.graph.mailSearchFolder",
  filterQuery: "contains(subject, 'Analytics')"
};

let res = await client.api('/me/mailFolders/AAMkAGVmMDEzM')
    .version('beta')
    .update({mailFolder : mailFolder});

```