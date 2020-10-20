---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2bed737e481026f7ddd432a45408982e207c4726
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608129"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contacts')
    .version('beta')
    .get();

```