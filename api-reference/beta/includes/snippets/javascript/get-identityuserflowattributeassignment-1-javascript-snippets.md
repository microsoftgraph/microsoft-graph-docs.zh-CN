---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 457cd8d39e6fc534733cd75907471581f0281e6b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944731"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userAttributeAssignments = await client.api('/identity/b2cUserFlows/{id}/userAttributeAssignments')
    .version('beta')
    .get();

```