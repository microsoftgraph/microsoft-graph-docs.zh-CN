---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b35048fed77db9fa40574bf5532019075c522f2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809973"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/print/taskDefinitions/92d72a3d-cad7-4809-8924-43833282b079/tasks')
    .version('beta')
    .get();

```