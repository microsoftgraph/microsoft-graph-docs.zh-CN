---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9598a010a9cceea09f5f096c8095b032e4cb190
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613874"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoleAssignments')
    .version('beta')
    .filter('isElevated eq true and expirationDateTime ne null or isElevated eq false')
    .get();

```