---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07d170544eae75b519fb6da232524e7ab8fb61b51fdb10e397345350785d2a68
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333748"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printTask = await client.api('/print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}')
    .get();

```