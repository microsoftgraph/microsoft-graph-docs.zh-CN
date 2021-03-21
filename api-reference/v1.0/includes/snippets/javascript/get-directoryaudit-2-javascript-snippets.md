---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9f76e55a331d6530cec037161397ce6d25fc4bf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956693"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryAudits = await client.api('/auditLogs/directoryAudits')
    .get();

```