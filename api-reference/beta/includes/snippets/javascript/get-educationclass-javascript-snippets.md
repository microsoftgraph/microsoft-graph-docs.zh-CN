---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af98064b6d8d0b45bb435863beafff942ac52716
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606779"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11023')
    .version('beta')
    .get();

```