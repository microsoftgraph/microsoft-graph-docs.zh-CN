---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a70bdc11967e30b239d0d64ba4c2b274409eea4f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738464"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id|userPrincipalName}/manager')
    .get();

```