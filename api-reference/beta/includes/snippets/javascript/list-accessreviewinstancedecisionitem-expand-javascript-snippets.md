---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c39a312e92ae1c87c34f234adbee561b2fc65f2
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63332849"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/identityGovernance/accessReviews/decisions/filterByCurrentUser(on='reviewer')')
    .version('beta')
    .expand('instance($expand=definition)')
    .get();

```