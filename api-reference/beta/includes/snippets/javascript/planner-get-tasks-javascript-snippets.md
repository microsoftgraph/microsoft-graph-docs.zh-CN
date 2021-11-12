---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10ed7c432e89a305a899dbdcd639c2cd75de7d642ec711f01fdd9108162f9478
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164187"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/planner/tasks')
    .version('beta')
    .get();

```