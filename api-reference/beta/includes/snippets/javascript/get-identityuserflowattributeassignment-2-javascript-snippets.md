---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6d803069707b127c1cf3ff9ad77d2b09b758779fe12e7542c0def8e7cc2be17
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105891"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userAttributeAssignments = await client.api('/identity/b2xUserFlows/{id}/userAttributeAssignments')
    .version('beta')
    .get();

```