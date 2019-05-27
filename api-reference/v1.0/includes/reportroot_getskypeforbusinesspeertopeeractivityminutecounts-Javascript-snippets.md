---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2a837ebf2fc312740036ecdb8cad250c4bbf9a89
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457395"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')')
    .get();

```