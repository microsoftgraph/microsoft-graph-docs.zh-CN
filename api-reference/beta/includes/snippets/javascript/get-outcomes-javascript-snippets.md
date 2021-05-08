---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75ad05a9ae2385c69db7034385b9005c47ce3933
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52254267"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let outcomes = await client.api('/education/classes/{id}/assignments/{id}/submissions/{id}/outcomes')
    .version('beta')
    .get();

```