---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e19da7b4487a42bf4737c144bae08e2e41c4cf7d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50768650"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/print/taskDefinitions/{taskDefinitionId}/tasks')
    .get();

```