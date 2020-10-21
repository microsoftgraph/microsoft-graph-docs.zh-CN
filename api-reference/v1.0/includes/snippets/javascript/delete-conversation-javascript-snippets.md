---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 295ff960fc47fd9a6836fbaeb9a3ac5877cf48cd
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611101"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/conversations/{id}')
    .delete();

```