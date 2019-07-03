---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ca884fea066ef5075fedfbb579c9e07be86bb557
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520664"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/endpoints')
    .version('beta')
    .get();

```