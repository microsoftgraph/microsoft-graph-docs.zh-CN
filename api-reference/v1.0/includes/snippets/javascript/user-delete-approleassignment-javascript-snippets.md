---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 933a34a10a0893a93155de9aedd76c1be732dd3d
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335031"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/appRoleAssignments/{id}')
    .delete();

```