---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e388c8069e83c674f288493a6ea372814527609e
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844825"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/b2cUserFlows/B2C_1_Customer/languages/en/defaultPages/idpselections/$value')
    .version('beta')
    .get();

```