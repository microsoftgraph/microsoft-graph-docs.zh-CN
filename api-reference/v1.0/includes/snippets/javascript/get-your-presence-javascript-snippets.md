---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 582454af0c5b9e4928440f115c9c101e5428811a
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663953"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/presence')
    .get();

```