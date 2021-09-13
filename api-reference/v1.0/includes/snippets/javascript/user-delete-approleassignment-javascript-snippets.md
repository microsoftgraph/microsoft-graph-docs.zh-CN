---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e224f0df749d19fb9d25615178c57035f51d5be319ac9e53a25bf4fbe0efdb1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164155"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/{id}/appRoleAssignments/{id}')
    .delete();

```