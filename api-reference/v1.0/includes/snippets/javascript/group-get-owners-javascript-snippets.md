---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 845b54100cd26bbf2984bddae5300bcf973307fe
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889065"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/owners')
    .get();

```