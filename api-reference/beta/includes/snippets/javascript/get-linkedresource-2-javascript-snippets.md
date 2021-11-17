---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf64362f17bebe30a45f185d499f0329b3cba79495fdbe3c5200c27c12cc3445
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333695"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let linkedResources = await client.api('/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources')
    .version('beta')
    .get();

```