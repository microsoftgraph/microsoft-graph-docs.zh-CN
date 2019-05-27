---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5d9e2e0685770083f6fa62a9cf9f4ab8d29891a4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459640"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendar')
    .delete();

```