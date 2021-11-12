---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89a9d7172ff0de532aa96b7a140acd0b73c8d50e5d8367d5614fdd5b1f90565b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164286"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/print/taskDefinitions/{taskDefinitionId}/tasks')
    .get();

```