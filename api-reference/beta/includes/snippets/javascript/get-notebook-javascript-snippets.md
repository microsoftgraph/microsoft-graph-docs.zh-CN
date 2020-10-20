---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c2a52c88a95be8edc48538767ff0bb5448f7faf
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605910"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/notebooks/{id}')
    .version('beta')
    .get();

```