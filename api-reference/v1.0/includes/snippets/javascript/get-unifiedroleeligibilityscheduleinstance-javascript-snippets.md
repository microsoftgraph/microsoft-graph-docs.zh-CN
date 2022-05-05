---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e3b484bea0602b67224ec32f551e3fc836abe93
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204892"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleEligibilityScheduleInstance = await client.api('/roleManagement/directory/roleEligibilityScheduleInstances/8MYkhImhnkm70CbBdTyW1BbHHAdHgZdDpbqyEFlRzAs-1-e')
    .get();

```