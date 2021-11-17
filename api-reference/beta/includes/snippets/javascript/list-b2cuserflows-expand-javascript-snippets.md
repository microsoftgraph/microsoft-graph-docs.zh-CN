---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2088e8d95945b4f0649d88af8428f80afa0c2c6af9de4a013a37a6c372a394f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219206"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let b2cUserFlows = await client.api('/identity/b2cUserFlows')
    .version('beta')
    .expand('identityProviders')
    .get();

```