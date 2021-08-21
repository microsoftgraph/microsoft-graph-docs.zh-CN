---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a5fb41208b2d0e299f85acb068fed53359677604b27ee3c45b771db6f190473
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220476"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleAssignmentScheduleInstance = await client.api('/roleManagement/directory/roleAssignmentScheduleInstances/eb18c026-c026-eb18-26c0-18eb26c018eb')
    .version('beta')
    .get();

```