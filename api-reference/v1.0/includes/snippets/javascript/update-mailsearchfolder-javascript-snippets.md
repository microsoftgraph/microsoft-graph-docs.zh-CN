---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a90e6c88c811125794ccbde23d924c7b7f65b3e1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732253"
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
    .update({mailFolder : mailFolder});

```