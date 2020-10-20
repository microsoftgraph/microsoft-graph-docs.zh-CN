---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9345fd73eb0d2f8a89876986544c4db22b5eae3c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614061"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/synchronizationProfiles/{id}/errors')
    .version('beta')
    .get();

```