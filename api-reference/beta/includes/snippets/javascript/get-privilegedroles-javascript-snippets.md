---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22f363a5a1360742f5d6f066e56e677fe796a54e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794482"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let privilegedRoles = await client.api('/privilegedRoles')
    .version('beta')
    .get();

```