---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6be689aeb4aecea93432ded2743c28ca194c5282a0e1bc63148f92bc46b9df2e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163889"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teamwork/workforceIntegrations/{workforceIntegrationId}')
    .version('beta')
    .delete();

```