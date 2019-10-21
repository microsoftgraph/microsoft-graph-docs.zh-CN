---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2bd88383bf2578903972219354f636a6d6a420ce
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "35705527"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}')
    .version('beta')
    .delete();

```