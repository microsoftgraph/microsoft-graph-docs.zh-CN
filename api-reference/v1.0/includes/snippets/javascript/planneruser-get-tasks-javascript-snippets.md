---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 510e638ace69a6dfbe7cad8332a38f0718d6c0a3
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "37637806"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/planner/tasks')
    .get();

```