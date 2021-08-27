---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71391acdc474c4fabe9d85ea1a2a60b6bd827f5406697cb3f3ae6a22d95142ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106899"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let availableProviderTypes = await client.api('/identity/identityProviders/availableProviderTypes')
    .version('beta')
    .get();

```