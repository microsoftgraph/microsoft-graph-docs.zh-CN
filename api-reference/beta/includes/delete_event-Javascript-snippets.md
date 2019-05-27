---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7ab3f924b99200170176403322dd53d13ba8da71
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438313"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/{id}')
    .version('beta')
    .delete();

```