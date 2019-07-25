---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 39f0d86ddf3e1ce9a5a79a29fb506d572460e147
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722396"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointActivityFileCounts(period='D7')')
    .get();

```