---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea30b8d409ab332fb712c512f7e5e98b007030a7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944735"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userAttributeAssignments = await client.api('/identity/b2cUserFlows/{id}/userAttributeAssignments')
    .version('beta')
    .expand('userAttribute')
    .get();

```