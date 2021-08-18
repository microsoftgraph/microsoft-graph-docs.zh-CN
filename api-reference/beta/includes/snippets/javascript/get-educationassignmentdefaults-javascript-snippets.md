---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c458a4d3d9540b3075208eaf287efc0d79e24ac6d72758ab8e1a576f1822c82
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332921"
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