---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ebae68427a214e25f8f96aeb4ca2a2db8d51f71
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794618"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sections = await client.api('/me/onenote/notebooks/{id}/sections')
    .version('beta')
    .get();

```