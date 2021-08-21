---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d2f111792cf28d1b595b20d084497a5fc18c766c5215e6fec4e887d0ec76b24
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219843"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleEligibilityScheduleInstance = await client.api('/roleManagement/directory/roleEligibilityScheduleInstances/5cfd7709-7709-5cfd-0977-fd5c0977fd5c')
    .version('beta')
    .get();

```