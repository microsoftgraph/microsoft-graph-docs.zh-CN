---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a759736b833de366421adaefa689f1989c2e59b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62098558"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const baseTaskList = {
    displayName: 'Shopping list'
};

await client.api('/me/tasks/lists')
    .version('beta')
    .post(baseTaskList);

```