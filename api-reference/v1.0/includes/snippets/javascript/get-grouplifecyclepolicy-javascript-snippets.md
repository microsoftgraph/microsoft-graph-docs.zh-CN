---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 63a3f59d6dd4323d7ec3ddf81a84a9967d4e7824
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722476"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groupLifecyclePolicies')
    .get();

```