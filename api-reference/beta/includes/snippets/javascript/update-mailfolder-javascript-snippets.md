---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 86021fd7e606eab6baf025d12852367fe04e4966
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729682"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: "displayName-value",
};

let res = await client.api('/me/mailFolders/AAMkAGVmMDEzM')
    .version('beta')
    .update({mailFolder : mailFolder});

```