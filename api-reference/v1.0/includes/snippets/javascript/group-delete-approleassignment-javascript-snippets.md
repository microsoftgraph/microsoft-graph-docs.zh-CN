---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5045900e1d9252ddb42b99095d148c56450a5900aaea009da78abeb52c347ce6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278557"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/appRoleAssignments/{id}')
    .delete();

```