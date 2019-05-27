---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f005c10702e009eafbc035f3b1d2147beca143ae
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474657"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/shares/{shareIdOrUrl}/driveItem')
    .version('beta')
    .expand('children')
    .get();

```