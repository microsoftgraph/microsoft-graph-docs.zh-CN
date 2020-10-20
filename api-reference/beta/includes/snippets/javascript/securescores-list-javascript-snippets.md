---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a7e0ea0abfa0c927ca9f913693fd85feb3a7559
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617670"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/secureScores')
    .version('beta')
    .top(1)
    .get();

```