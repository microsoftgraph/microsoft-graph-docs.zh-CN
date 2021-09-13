---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e75c631ba86332ae6da4eca736a5bb4ff9529fe90ad4a1e0ffe37d4b61169fe2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277872"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/planner/tasks')
    .get();

```