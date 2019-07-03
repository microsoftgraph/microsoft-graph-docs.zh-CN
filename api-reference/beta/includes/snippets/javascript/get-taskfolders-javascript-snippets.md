---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a70506e89b600190f625644e876aa3dc9ec24ed8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521286"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/taskFolders')
    .version('beta')
    .get();

```