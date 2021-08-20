---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e6cd9c17c0ebc94bf9d4bdae2f162e11439b4c7e55bc25ad3b57a080b198296
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332504"
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