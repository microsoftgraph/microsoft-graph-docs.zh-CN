---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5595a128b9d337243ddd0b03f4bdeccb1fcc5344db0772d69aa675ec445bedd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162494"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/appRoleAssignments/{id}')
    .version('beta')
    .delete();

```