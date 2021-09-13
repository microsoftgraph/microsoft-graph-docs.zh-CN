---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02ec368101bb2a8141e781817517d383512ea38e2f87feede2eea2bd182e07b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220924"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/planner/tasks/{id}')
    .delete();

```