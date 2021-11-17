---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56eb35d29abc17b3cfa2540fd5239e3175428f9794bd9ab6cae3f3322ba875c9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221072"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delegatedPermissionClassifications = await client.api('/servicePrincipals/{id}/delegatedPermissionClassifications')
    .version('beta')
    .get();

```