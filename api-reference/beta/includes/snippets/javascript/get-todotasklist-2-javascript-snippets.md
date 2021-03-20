---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 232c794d2a67d3ce95f1b46195cdda42085f5cad
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953849"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let todoTaskList = await client.api('/me/todo/lists/AAMkADIyAAAAABrJAAA=')
    .version('beta')
    .get();

```