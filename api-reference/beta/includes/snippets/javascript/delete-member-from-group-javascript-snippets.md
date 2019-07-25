---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0789a1b03208a0b5505b19a1ecb0a842192a689f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858924"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/members/{id}/$ref')
    .version('beta')
    .delete();

```