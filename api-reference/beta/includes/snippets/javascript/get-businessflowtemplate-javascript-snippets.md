---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99cc4142fd1fc9a2f720615728a6f780de6fec97
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606529"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/businessFlowTemplates')
    .version('beta')
    .get();

```