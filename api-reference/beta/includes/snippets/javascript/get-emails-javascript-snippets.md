---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f102e53bece8b8d53af5b70600b64e6df8aa42e1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803129"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let emails = await client.api('/me/profile/emails')
    .version('beta')
    .get();

```