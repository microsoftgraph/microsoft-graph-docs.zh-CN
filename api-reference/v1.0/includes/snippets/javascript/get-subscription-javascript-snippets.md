---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75ad6a4201eb2637de33a2cf5e42e5bd4d8bd7c0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807690"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let subscription = await client.api('/subscriptions/{id}')
    .get();

```