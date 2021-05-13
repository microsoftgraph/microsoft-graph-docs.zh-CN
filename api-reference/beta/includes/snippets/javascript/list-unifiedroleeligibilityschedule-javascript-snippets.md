---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e38c1945a346a4292ca588b131e37186deb66744
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475306"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleEligibilitySchedules = await client.api('/roleManagement/directory/roleEligibilitySchedules')
    .version('beta')
    .get();

```