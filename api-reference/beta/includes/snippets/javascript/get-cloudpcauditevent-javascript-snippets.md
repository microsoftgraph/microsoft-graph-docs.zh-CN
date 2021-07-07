---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a56835fa6cad4a0d2be22796dd1689fc8737bdf5
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316879"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcAuditEvent = await client.api('/deviceManagement/virtualEndpoint/auditEvents/{id}')
    .version('beta')
    .get();

```