---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8241e650f5877d35d8f72968e9dc265d4ed8987
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "37995484"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schema = {
  baseType: "microsoft.graph.externalFile"
};

let res = await client.api('/connections/contosofiles/schema')
    .version('beta')
    .post(schema);

```