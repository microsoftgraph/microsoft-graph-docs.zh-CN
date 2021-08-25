---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce605f1e1cd97084eb48687ee1c185361c94b1e7
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58516056"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleEligibilityScheduleInstance = await client.api('/roleManagement/directory/roleEligibilityScheduleInstances/UafX_Qu2SkSYTAJlL-j6HCssmvzcHW1IohFf6Mp3-h9xbmLcN0jrQL5KvCnYihF4-2-e')
    .version('beta')
    .get();

```