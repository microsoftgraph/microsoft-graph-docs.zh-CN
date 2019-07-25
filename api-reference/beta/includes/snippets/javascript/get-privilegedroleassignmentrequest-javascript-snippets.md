---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5ebf9a83d435ab2146ce78e4f6cefa9488fb215a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720171"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoleAssignmentRequests')
    .version('beta')
    .get();

```