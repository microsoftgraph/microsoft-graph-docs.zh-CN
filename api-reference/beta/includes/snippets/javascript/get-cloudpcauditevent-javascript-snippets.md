---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98cc34b57ce9c4e1380f9a9dc9697576c2a227efd725e743c0e5bc0175f7ff5a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220941"
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