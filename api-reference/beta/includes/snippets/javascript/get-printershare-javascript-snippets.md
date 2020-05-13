---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ad9dbf971963a23617ccf61f911bd69262fbf28
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44216873"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/shares/{id}')
    .version('beta')
    .get();

```