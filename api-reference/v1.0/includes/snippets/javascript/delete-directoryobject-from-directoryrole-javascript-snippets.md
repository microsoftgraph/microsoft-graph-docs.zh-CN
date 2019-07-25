---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f967ac07ded10f92892dbec3926a8532c86aa745
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734031"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles/{id}/members/{id}/$ref')
    .delete();

```