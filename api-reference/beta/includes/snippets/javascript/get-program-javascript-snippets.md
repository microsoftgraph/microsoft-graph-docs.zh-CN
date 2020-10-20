---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b99c3dff2098cae61f03ffefe988bfa660cc84b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606581"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/programs')
    .version('beta')
    .get();

```