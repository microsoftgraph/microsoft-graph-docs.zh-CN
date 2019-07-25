---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b183f4b88f7880a014eb93726c63ba3a9aad62f7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860264"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/schools/10002/users')
    .version('beta')
    .get();

```