---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dada5aea392a588d3791c1175ef6fd55675b75aa
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475145"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleAssignmentSchedules = await client.api('/roleManagement/directory/roleAssignmentSchedules')
    .version('beta')
    .get();

```