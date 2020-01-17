---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf67a02ac51cdc07026e96c019411df0ba2f1075
ms.sourcegitcommit: 844c6d552a8a60fcda5ef65148570a32fd1004bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/17/2020
ms.locfileid: "41225095"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists/{list-id}?$select=name,lastModifiedDateTime&$expand=columns($select=name,description),items($expand=fields($select=Name,Color,Quantity))')
    .version('beta')
    .get();

```
