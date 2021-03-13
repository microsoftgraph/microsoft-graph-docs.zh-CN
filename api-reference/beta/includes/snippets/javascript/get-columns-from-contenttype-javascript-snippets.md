---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aad9801ef84f38136d222c3418052fbcfd694f50
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770531"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let columns = await client.api('/sites/{site-id}/contentTypes/{contentType-id}/columns')
    .version('beta')
    .get();

```