---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 544a3560d37a5277b5e0728a335e3d4015df1f16
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802655"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let list = await client.api('/sites/{site-id}/lists/{list-title}')
    .version('beta')
    .get();

```