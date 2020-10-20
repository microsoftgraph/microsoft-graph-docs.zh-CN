---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34873fe95c0657fb6f715084df0ce43cb77970a4
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618300"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/threads/{id}')
    .version('beta')
    .delete();

```