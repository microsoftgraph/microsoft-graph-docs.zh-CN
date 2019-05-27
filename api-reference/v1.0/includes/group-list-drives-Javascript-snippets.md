---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f8a20e9595a24006fa5c006e4ede9cc966219f08
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478137"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{groupId}/drives')
    .get();

```