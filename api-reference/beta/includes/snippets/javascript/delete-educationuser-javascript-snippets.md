---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c58804f8215d3d90dfc528d22d554e5c819f12e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611695"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/users/13019')
    .version('beta')
    .delete();

```