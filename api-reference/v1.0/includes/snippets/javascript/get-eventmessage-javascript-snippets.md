---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7f643262fae0c9435c5a485697328772d763fe97
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735061"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkADYAAAImV_lAAA=')
    .get();

```