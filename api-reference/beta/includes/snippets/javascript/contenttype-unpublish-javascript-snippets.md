---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a22b11a398d09cff5b5fffbb0bd84ca1eea0773f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773359"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/sites/{siteId}/contentTypes/{contentTypeId}/unpublish')
    .version('beta')
    .post();

```