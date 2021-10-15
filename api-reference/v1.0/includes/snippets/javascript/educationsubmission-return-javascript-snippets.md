---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 931c986b34544dbfcb8903854770a3531862abf3
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60365794"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/7192332b-e904-4891-81e2-356242ab1858/submissions/022fb52d-1278-d21f-e827-2221a6a3e516/return')
    .post();

```