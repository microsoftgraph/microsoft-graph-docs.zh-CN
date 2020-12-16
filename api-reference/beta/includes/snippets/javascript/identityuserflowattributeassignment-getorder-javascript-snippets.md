---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cce1b4e678c921301a10486c1e49c9d585887f2f
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689246"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/b2cUserFlows/{id}/userAttributeAssignments/getOrder')
    .version('beta')
    .get();

```