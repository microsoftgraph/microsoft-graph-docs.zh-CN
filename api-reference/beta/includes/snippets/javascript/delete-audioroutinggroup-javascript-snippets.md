---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 41ee69e2efdbcca998c34cfac20edfafcec64437
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710004"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/app/calls/{id}/audioRoutingGroups/{id}')
    .version('beta')
    .delete();

```