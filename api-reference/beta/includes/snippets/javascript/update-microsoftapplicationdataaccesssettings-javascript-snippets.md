---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12f6a5e07a7b94305e75f5c11f2791f5d199b0cb
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212413"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const microsoftApplicationDataAccessSettings = {
  disabledForGroup: 'edbfe4fb-ec70-4300-928f-dbb2ae86c981'
};

await client.api('/organization/{organizationId}/settings/microsoftApplicationDataAccess')
    .version('beta')
    .update(microsoftApplicationDataAccessSettings);

```