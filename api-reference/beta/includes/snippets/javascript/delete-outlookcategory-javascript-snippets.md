---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 714c0ec59ae4c48376b3707e8e726e06590a5e3a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720984"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8')
    .version('beta')
    .delete();

```