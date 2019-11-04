---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76504af0c527957f2fef1743c83c5dd75e606dbd
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936738"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/conditionalAccess/policies/{id}')
    .version('beta')
    .get();

```