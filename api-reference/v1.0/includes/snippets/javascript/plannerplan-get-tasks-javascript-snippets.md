---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f5c4cd7377715bc1b6947481cd44cf70242bcfa
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "37637833"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/plans/{plan-id}/tasks')
    .get();

```