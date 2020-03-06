---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f5c4cd7377715bc1b6947481cd44cf70242bcfa
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
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