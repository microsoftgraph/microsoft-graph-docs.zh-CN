---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f61553b3b8102b3016ae8e4a5c7f5216a9dfe2cf
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59508219"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/directory/deletedItems/microsoft.graph.group')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .select('id,displayName,deletedDateTime')
    .orderby('deletedDateTime asc')
    .get();

```