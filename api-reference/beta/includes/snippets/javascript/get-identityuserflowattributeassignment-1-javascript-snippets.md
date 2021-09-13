---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ca846a6151318291a53d0bd239a0f31d5cbae8761ff4597eb196acd98f997fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215918"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userAttributeAssignments = await client.api('/identity/b2cUserFlows/{id}/userAttributeAssignments')
    .version('beta')
    .get();

```