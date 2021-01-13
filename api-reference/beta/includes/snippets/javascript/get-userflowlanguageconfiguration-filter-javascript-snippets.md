---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63510ca39f9851b0b8bb2140ec3a55438dabd2f5
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844097"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages')
    .version('beta')
    .filter('isEnabled eq true')
    .get();

```