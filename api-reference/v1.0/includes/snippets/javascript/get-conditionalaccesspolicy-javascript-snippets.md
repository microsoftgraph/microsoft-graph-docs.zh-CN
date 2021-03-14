---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f8787f1d31220fa850cd4ce1a9683337529308c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796647"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conditionalAccessPolicy = await client.api('/identity/conditionalAccess/policies/{id}')
    .get();

```