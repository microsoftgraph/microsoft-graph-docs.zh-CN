---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18e9752e6d1d2baa97f4b805c04f4be16fab90e5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787340"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/drive/root/delta')
    .version('beta')
    .get();

```