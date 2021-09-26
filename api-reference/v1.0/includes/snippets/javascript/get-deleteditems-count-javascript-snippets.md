---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a449fbbe6ae174c94de12270f50ff34b4d805c2f
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767259"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/directory/deletedItems/microsoft.graph.group')
    .header('ConsistencyLevel','eventual')
    .select('id,displayName,deletedDateTime')
    .orderby('deletedDateTime asc')
    .get();

```