---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47abdb1a1d426829eb65dbe213f2280ba820e6e9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615874"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/licenseDetails')
    .version('beta')
    .get();

```