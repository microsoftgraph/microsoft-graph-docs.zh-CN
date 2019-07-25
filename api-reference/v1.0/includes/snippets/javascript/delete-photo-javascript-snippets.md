---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 099833c2dbc1cc9a956f1c4185e83f9e793748d1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732786"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id|userPrincipalName}/photo')
    .delete();

```