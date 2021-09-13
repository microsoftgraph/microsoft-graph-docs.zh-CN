---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d5d6948f271896596a9aa96f180f764d7f39386b403d65f0b499c7ec86ab74a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106032"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/planner/plans/{plan-id}/tasks')
    .get();

```