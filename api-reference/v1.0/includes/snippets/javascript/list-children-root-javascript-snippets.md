---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b570d2a9f4a6ba2066c54c40be4e9c2beef7b9d4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793372"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let children = await client.api('/me/drive/root/children')
    .get();

```