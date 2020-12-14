---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0ef3a38c402a50655a50e06ecebf77f62d82f2d
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657007"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/teamwork/installedApps/{id}/chat')
    .get();

```