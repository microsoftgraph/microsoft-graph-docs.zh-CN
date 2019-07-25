---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fdcaa49e6ac75c2c1e9bb4060ea7a28208a92ce1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714934"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me')
    .get();

```