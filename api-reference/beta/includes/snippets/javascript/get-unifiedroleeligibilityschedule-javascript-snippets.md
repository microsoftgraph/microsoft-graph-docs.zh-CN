---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2760eb72626d850c19352ea2553bb5701293969a
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58516045"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleEligibilitySchedule = await client.api('/roleManagement/directory/roleEligibilitySchedules/313af44a-07c9-43a7-9970-5072a6b5591f')
    .version('beta')
    .get();

```