---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 73d3f6f34a91250558f4d13e3a323198a7a46b15
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449739"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendar = {
  name: "Social events"
};

let res = await client.api('/me/calendar')
    .update({calendar : calendar});

```