---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad60e5ed939d9a477a3be9cf60a7e80c7d1cc4c7
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44216838"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/shares/{id}/allowedGroups')
    .version('beta')
    .get();

```