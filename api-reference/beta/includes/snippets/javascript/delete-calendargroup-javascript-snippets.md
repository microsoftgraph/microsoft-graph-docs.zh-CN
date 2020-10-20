---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 735477a1c584483fe940b60f40fd0f62b86c0744
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617493"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarGroups/{id}')
    .version('beta')
    .delete();

```