---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3c31a90697c38a852017ea9acc45af1d9fb14722
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730281"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/planner/all/delta')
    .version('beta')
    .get();

```