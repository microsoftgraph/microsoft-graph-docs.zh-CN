---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9a45ad8babe35c5f5e4fa9e022b908cfd680231
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657061"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/reopen')
    .version('beta')
    .post();

```