---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdf50955d804b8f1ae658632225e2bf6b9bd3e48
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773646"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationAssignmentSettings = await client.api('/education/classes/{id}/assignmentSettings')
    .version('beta')
    .get();

```