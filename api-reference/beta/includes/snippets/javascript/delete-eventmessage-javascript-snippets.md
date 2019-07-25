---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 09be6cce37496400b52c3e4798f2d33113feec0b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714053"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}')
    .version('beta')
    .delete();

```