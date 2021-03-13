---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 692a5cc64245014dae0dcd29cebfcd60650fa4fa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783122"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationRubric = await client.api('/education/me/assignments/{id}/rubric')
    .version('beta')
    .get();

```