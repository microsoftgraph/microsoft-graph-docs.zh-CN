---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ea9752e6f41d31327f2d610604809cfabe032cf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778677"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let reviewSet = await client.api('/compliance/ediscovery/cases/6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d/reviewSets/0157910c-57ce-4e48-bd4b-90f3c88ca32e')
    .version('beta')
    .get();

```