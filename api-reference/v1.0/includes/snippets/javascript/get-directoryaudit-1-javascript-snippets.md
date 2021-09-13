---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17592b64d1e7553cf460d78481d1adafcf3e3b2d2ed5b3e7f948533d6251097d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277188"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryAudit = await client.api('/auditLogs/directoryAudits/{id}')
    .get();

```