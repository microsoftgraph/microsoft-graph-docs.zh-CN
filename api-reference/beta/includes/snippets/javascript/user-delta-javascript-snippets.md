---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bfdbca0a0c81b8b40fa01d5c0c205f4262e5f9de
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604265"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/delta')
    .version('beta')
    .get();

```