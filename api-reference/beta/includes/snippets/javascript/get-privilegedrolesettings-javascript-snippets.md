---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 307b8a1fea1c2125623bda708bbb097263b238c9915314462f4a855b0f45d085
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333665"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let privilegedRoleSettings = await client.api('/privilegedRoles/{id}/settings')
    .version('beta')
    .get();

```