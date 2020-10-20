---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c31a90697c38a852017ea9acc45af1d9fb14722
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617496"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/planner/all/delta')
    .version('beta')
    .get();

```