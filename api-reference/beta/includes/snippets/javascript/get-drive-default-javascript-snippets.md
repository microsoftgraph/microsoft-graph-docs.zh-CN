---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 308c9270f584c97176a4eb6b305a46590eb29f5a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706483"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive')
    .version('beta')
    .get();

```