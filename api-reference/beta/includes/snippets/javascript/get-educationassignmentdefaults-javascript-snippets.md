---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a8bc2ac63ce80311267c3a51e5e4d4cd4c2db1d
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507405"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationAssignmentDefaults = await client.api('/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignmentDefaults')
    .version('beta')
    .get();

```