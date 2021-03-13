---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58f68d7fafd3af9bb6de1066c402b62012798b7d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795700"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/education/users')
    .version('beta')
    .get();

```