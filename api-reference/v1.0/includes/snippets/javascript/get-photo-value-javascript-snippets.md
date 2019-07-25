---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6cff5b6caf4c77ccf9e65cc8cc568bf9b0cf1111
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733357"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id|userPrincipalName}/photo/$value')
    .get();

```