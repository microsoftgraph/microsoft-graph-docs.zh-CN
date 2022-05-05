---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6f6f95ae34facb2b96fcbd8e2f51f5e2c9184f0
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205703"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let microsoftApplicationDataAccessSettings = await client.api('/organization/{organizationId}/settings/microsoftApplicationDataAccess')
    .version('beta')
    .get();

```