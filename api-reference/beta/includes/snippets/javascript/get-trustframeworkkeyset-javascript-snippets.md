---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b264016180e0b12012873036f7336d07a399a3f2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799246"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let trustFrameworkKeySet = await client.api('/trustFramework/keySets/{id}')
    .version('beta')
    .get();

```