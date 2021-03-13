---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21c02989a6b0b73fb664a924a2c845b11741b7bd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797929"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/mailFolders/delta')
    .version('beta')
    .get();

```