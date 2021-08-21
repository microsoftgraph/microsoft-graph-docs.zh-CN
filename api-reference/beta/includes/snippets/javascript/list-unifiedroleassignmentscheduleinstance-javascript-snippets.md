---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2afd1e7382b7f29c9b9245b8aa442a083fdd0507643ee1a67c5c1058535071e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158450"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleAssignmentScheduleInstances = await client.api('/roleManagement/directory/roleAssignmentScheduleInstances')
    .version('beta')
    .get();

```