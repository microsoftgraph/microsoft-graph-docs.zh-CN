---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 961abf87d514e6716d1e34c0127231b3e7fb48cd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34470175"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/special/{name}')
    .get();

```