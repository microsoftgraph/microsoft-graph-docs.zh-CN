---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc9ba51c14d3c3822f0210a142343a60d338226303439c98c4808d4043caea64
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104498"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/b2cUserFlows/{id}')
    .version('beta')
    .delete();

```