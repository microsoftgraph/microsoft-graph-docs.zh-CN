---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bc2a79a29ef237d77d5358e3e419053439daf005add9acdc3d266811d321027
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162700"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleManagementPolicies = await client.api('/policies/roleManagementPolicies')
    .version('beta')
    .get();

```