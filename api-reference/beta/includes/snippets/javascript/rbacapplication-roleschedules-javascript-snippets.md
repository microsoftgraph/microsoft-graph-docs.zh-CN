---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5e01de48e48d8b1ced4e65a6d8845a611ae8489
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474682"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleSchedules = await client.api('/roleManagement/directory/roleSchedules(directoryScopeId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',appScopeId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',principalId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',roleDefinitionId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea')')
    .version('beta')
    .get();

```