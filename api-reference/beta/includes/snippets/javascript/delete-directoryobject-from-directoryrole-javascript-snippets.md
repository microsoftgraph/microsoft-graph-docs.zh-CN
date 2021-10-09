---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ad7d8398eb0899d0b88885455af18108f457d8ec45c6109b72ad057c1e5dae9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220826"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/directoryRoles/f8e85ed8-f66f-4058-b170-3efae8b9c6e5/members/bb165b45-151c-4cf6-9911-cd7188912848/$ref')
    .version('beta')
    .delete();

```