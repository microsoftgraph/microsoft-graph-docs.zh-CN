---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e95c92eaf6ee776f61a8e22a38faec366e4e5918
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938039"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/userFlows/{id}')
    .version('beta')
    .delete();

```