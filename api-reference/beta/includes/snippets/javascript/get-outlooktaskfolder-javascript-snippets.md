---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c1fd4bdf1ebcb03f949f6e7b8631b618734c7ec
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609835"
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