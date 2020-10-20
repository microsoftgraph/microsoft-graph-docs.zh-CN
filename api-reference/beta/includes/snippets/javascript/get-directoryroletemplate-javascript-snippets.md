---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e37f8fbd82bc98a1fb801bd2a32881c79560756c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616046"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoleTemplates/{id}')
    .version('beta')
    .get();

```