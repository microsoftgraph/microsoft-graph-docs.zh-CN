---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a8eb27c85095aa79fa89c8dbff276af017dccf885ba4390818c57c1748178f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328948"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerTaskDetails = await client.api('/planner/tasks/{task-id}/details')
    .get();

```