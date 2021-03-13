---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2da6ff7ee0adcba7a740ccda63f90d0067cb0246
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795048"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationAssignmentDefaults = await client.api('/education/classes/{id}/assignmentDefaults')
    .version('beta')
    .get();

```