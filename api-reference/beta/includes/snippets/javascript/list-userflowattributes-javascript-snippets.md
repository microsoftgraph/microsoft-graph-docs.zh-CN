---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0f6958e3c708e8d909e8c86b6875c56e79ab6036140a6203adf9ca1363e1678
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163975"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userFlowAttributes = await client.api('/identity/userFlowAttributes')
    .version('beta')
    .get();

```