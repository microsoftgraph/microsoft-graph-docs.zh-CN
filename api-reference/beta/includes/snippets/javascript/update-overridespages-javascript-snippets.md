---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c6e966bc1457378ea53f797ec9fe1540a330379
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844795"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const stream = {
  LocalizedStrings: [
        {
            ElementType: "UxElement",
            ElementId: null,
            StringId: "alert_message",
            Override: true,
            Value: "Are you sure that you want to cancel your selection?"
        }
    ]
};

let res = await client.api('/identity/b2cUserFlows/B2C_1_Customer/languages/en/overridesPages/phonefactor/$value')
    .version('beta')
    .put(stream);

```