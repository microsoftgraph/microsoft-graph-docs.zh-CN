---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 72ad36680fecb8077ba87c62591dcdb6570a9aaf
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636662"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookCategory = {
      displayName:"Project expenses",
      color:"preset9"
};

let res = await client.api('/me/outlook/masterCategories')
    .version('beta')
    .post(outlookCategory);

```