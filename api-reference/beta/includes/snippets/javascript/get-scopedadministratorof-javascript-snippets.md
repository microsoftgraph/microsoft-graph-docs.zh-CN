---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 97b7984ee950eb99b206296337f65b7cbaaddadf
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521409"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/scopedAdministratorOf')
    .version('beta')
    .get();

```