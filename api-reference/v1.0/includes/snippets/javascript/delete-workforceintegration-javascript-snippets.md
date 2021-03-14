---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d82c426ca42a2cbb3d5abd36963e563c26f1a6f1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780337"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teamwork/workforceIntegrations/{workforceIntegrationId}')
    .delete();

```