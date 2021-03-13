---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e750d8060472e8e8e97ee3d2c21ea0c89cb20b00
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773436"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printTask = await client.api('/print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}')
    .get();

```