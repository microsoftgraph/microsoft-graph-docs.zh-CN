---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c94d65df20f17312290a4aeda7c8dfc8042f2f5a
ms.sourcegitcommit: 844c6d552a8a60fcda5ef65148570a32fd1004bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/17/2020
ms.locfileid: "41225093"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists/{list-id}?$select=id,name,lastModifiedDateTime&$expand=columns($select=name,description),items($expand=fields($select=Name,Color,Quantity))')
    .get();

```
