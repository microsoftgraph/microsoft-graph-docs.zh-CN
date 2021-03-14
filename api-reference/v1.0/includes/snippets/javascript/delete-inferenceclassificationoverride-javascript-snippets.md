---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8265865eb34eb82364d7b654b587e08936d38824
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790587"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r')
    .delete();

```