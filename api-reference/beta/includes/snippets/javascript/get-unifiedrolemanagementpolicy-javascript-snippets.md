---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae0871656a5c909f6f0f8fad65643cf08afa4caa
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475061"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleManagementPolicy = await client.api('/policies/roleManagementPolicies/f93a5c37-5c37-f93a-375c-3af9375c3af9')
    .version('beta')
    .get();

```