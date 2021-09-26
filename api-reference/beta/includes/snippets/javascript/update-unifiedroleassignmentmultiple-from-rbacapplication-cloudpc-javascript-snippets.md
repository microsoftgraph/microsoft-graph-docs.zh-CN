---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6de00535c37502c801dbc22f214ec2d7aaaa37302e5dd919e3c2d4fc41bf8283
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220059"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleAssignmentMultiple = {
    displayName: 'NewName',
    description: 'A new roleAssignment'
};

await client.api('/roleManagement/cloudPC/roleAssignments/dbe9d288-fd87-41f4-b33d-b498ed207096')
    .version('beta')
    .update(unifiedRoleAssignmentMultiple);

```