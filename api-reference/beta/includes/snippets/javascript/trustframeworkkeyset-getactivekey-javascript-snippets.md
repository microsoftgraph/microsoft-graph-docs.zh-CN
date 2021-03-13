---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdddd1bce6dae98f8a89b5586cc37c1c6df34cb8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791895"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let trustFrameworkKey = await client.api('/trustFramework/keySets/{id}/getActiveKey')
    .version('beta')
    .get();

```