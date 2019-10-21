---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1abbf9a9de03b976ec4f3afaefaba04043ec83d7
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "36413477"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/buckets/{id}')
    .version('beta')
    .delete();

```