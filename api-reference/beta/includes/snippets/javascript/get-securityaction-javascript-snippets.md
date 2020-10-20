---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1f58c2ab4589b30baa76c858503dea8a843d354
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606082"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/securityActions/{id}')
    .version('beta')
    .get();

```