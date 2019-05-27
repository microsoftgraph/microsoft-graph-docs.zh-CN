---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ea179d374485013d5537d50b9efcc13666454240
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34435919"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/pages')
    .version('beta')
    .get();

```