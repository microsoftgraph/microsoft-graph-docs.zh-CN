---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e9598a010a9cceea09f5f096c8095b032e4cb190
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499841"
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