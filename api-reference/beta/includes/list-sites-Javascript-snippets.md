---
description: 自动生成的文件。 不修改
ms.openlocfilehash: daceffe89c908f9bfb6562b8f3ec57dc6e817499
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444396"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites')
    .version('beta')
    .filter('siteCollection/root ne null')
    .get();

```