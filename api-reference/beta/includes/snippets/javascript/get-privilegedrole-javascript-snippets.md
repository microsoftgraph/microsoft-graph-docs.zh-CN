---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e5f4e1e8ed9d0556954a0042ce3a55350e1685146eb3a4b38edcc8a4381de45
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105996"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let privilegedRole = await client.api('/privilegedRoles/{id}')
    .version('beta')
    .get();

```