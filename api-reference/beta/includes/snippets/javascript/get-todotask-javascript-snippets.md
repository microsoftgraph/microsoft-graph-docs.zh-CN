---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6835bdda0d5902d3caa5276e337a85b624772019
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873177"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/todo/lists/35e2-35e2-721a-e235-1a72e2351a7/tasks')
    .version('beta')
    .get();

```