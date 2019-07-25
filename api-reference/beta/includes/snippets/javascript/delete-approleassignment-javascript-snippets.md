---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7ced80c309a7cc3e81f58df5777061d9152d05ab
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710035"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/appRoleAssignments/{id}')
    .version('beta')
    .delete();

```