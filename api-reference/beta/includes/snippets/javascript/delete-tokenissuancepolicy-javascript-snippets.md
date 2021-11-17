---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c0c564b419b6a69f024030f8faab468a409f4569e2d5ee94aa9c7bc90bb591f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903625"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/tokenIssuancePolicies/{id}')
    .version('beta')
    .delete();

```