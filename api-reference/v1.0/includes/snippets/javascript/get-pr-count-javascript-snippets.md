---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ebc2ccf95c140147471c1d4593dbd8ce0fc63e1
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903662"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/members/microsoft.graph.user')
    .header('ConsistencyLevel','eventual')
    .search('displayName:Pr')
    .select('displayName,id')
    .orderby('displayName ')
    .get();

```