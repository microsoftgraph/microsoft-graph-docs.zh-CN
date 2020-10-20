---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3fb8aa55d6ea5af1347404dff8f1fef8312cb98d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608788"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoleAssignments/{id}')
    .version('beta')
    .get();

```