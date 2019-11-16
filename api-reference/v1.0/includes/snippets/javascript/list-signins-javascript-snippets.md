---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6bf1bcbc9767c9212ac1e15b5d3344351910928
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "35734082"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/auditLogs/signIns')
    .get();

```