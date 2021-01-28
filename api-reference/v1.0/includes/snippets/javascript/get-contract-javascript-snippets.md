---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab311af8f209d46553cd574ea8a5e28e24c6b6e1
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015604"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contracts/{id}')
    .get();

```