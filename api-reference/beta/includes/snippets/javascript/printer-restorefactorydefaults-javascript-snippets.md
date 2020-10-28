---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 928265691a028031b009bf37f38148ea9914a664
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782744"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/printers/{id}/restoreFactoryDefaults')
    .version('beta')
    .post();

```