---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95c3e84a9972764b94c039fb9ec8724a5dd72d80
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793587"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/devices/{id}')
    .delete();

```