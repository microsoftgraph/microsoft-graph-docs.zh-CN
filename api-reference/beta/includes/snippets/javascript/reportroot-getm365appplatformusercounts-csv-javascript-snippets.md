---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0f6f37fe5311d691aec3dbf742e64d696ed36e0
ms.sourcegitcommit: 7dcd32f9e959bea2dfd81d9e0d4092f93da43cb7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2020
ms.locfileid: "46657966"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getM365AppPlatformUserCounts(period='D7')/content')
    .version('beta')
    .get();

```