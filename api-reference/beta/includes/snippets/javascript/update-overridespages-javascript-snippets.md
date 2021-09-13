---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db12a3849599ad759880dc54bcf9404ac7ff739ddcea6c25bcff65c3414b5d4e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221290"
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