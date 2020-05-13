---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d7d191ec20d396bd4d4e648c86e0fb818eb1842
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44216957"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/shares')
    .version('beta')
    .get();

```