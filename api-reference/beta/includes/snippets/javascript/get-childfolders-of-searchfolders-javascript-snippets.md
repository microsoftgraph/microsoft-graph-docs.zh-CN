---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6d2488ce8ef0a8e0afd944ab044c0c981be38d5c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729773"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/searchfolders/childFolders')
    .version('beta')
    .get();

```