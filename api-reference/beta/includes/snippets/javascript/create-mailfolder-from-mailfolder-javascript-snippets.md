---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 508db2f1f43b92aaf1c7d4d9eb07ea978a2cdfa1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721607"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: "displayName-value",
};

let res = await client.api('/me/mailFolders/{id}/childFolders')
    .version('beta')
    .post({mailFolder : mailFolder});

```