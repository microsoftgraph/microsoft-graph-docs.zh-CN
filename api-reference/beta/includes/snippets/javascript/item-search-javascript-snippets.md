---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35948e23d6cb3c5d47a5a82c321c00b237092eb5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809869"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let search = await client.api('/me/drive/root/search(q='Contoso Project')')
    .version('beta')
    .get();

```