---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 915ab48253c3ccf7695bad173a9cedd09caf42ae
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657193"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/teamwork/installedApps/{id}/chat')
    .version('beta')
    .get();

```