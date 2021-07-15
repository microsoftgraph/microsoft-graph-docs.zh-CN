---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d46789e00db1ae2ffb92e19c78cd18605fd05472
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442677"
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