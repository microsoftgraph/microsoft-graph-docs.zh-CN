---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 18e9c0c350eb5adeb3bcd9e6979994314428c693
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454388"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/activities/recent')
    .get();

```