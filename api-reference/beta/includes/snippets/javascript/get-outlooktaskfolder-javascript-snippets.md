---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5c1fd4bdf1ebcb03f949f6e7b8631b618734c7ec
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720893"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/taskFolders/AAMkADIyAAAAABrJAAA=')
    .version('beta')
    .get();

```