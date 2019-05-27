---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6a6abdaee2ea42cefdd9f63cbda04b38ecfcb49e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449039"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contacts/{id}/manager')
    .version('beta')
    .get();

```