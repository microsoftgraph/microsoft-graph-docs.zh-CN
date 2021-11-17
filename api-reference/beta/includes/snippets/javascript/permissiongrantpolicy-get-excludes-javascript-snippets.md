---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c76f34303de738317b6dc9d259413929fdc3675cd66d00dca7dd85a23b3bc44
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903502"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let excludes = await client.api('/policies/permissionGrantPolicies/microsoft-application-admin/excludes')
    .version('beta')
    .get();

```