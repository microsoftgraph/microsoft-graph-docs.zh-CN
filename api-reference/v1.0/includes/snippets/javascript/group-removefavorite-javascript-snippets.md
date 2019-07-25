---
description: 自动生成的文件。 不修改
ms.openlocfilehash: affc1001ae55c71c5b7c94d333311a9d71296cc1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722685"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/removeFavorite')
    .post();

```