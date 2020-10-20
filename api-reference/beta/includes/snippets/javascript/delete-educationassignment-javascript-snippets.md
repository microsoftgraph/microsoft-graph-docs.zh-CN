---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12daaa229d9f88558c1b38dd1797966e5e690696
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621136"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11014/assignmentCategories/19002')
    .version('beta')
    .delete();

```