---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4e22c4464c2f52d18f437b1b9f7c775fd9aad1c7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451950"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/renew')
    .post();

```