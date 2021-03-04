---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 915e8029476d8e8232c738b9094e1c5f3e5dd463
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "50435157"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/b2xUserFlows/{id}/userAttributeAssignments')
    .version('beta')
    .expand('userAttribute')
    .get();

```