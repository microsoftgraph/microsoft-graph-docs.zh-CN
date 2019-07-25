---
description: 自动生成的文件。 不修改
ms.openlocfilehash: de4951d8c8ef3a2db535146aefbaea2cbda803b5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877982"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contacts/{id}/memberOf')
    .version('beta')
    .get();

```