---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0780a954208438e9fd60076f510ae345bb825709
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436122"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists/{list-id}')
    .version('beta')
    .get();

```