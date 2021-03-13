---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bfdcdd3d404ce4b517a3b12f432fea54333e4f0c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782092"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let settings = await client.api('/me/analytics/settings')
    .version('beta')
    .get();

```