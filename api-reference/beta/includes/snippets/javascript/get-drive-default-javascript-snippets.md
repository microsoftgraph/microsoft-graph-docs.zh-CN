---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1dfe65f8d2a4897909f6d6a83e63ef28807119b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795578"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drive = await client.api('/me/drive')
    .version('beta')
    .get();

```