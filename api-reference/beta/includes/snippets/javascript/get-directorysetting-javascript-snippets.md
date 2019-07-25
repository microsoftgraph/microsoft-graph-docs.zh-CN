---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fb0bf591b2591a0104e6ceee5b0451e9f1075c5f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713289"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/settings/{id}')
    .version('beta')
    .get();

```