---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 508db2f1f43b92aaf1c7d4d9eb07ea978a2cdfa1
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466442"
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