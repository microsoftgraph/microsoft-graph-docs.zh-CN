---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab690e8fda953cfacd82f3dad419ef960409b2b2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804746"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const stream = {
  LocalizedStrings: [
        {
            ElementType: 'UxElement',
            ElementId: null,
            StringId: 'alert_message',
            Override: true,
            Value: 'Are you sure that you want to cancel your selection?'
        }
    ]
};

await client.api('/identity/b2cUserFlows/B2C_1_Customer/languages/en/overridesPages/phonefactor/$value')
    .version('beta')
    .put(stream);

```