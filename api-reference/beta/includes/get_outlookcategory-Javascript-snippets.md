---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 57240431ab24cf36f183300d9422242dacbf2b0b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448130"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/masterCategories/de912e4d-c790-4da9-949c-ccd933aaa0f7')
    .version('beta')
    .get();

```