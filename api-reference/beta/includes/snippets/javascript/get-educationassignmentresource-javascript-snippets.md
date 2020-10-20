---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a70301ef31df363efb6c2bca1a092b191161a0e6
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614112"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11021/assignments/19002/resources/22002')
    .version('beta')
    .get();

```