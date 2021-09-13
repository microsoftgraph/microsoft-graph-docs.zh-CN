---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6fc92548513a40f5f7ce8b2383c73a4e65e51489f84a6a0016c2e64a210f40ff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277585"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
  allowEmailVerifiedUsersToJoinOrganization: false
};

await client.api('/policies/authorizationPolicy')
    .update(authorizationPolicy);

```