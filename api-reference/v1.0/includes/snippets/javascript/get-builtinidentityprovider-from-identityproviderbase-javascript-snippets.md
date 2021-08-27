---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efbbc44cdc27cfc6ada79de5af15c684d58dd67401649cb364f7dc2d10d49bed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409539"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviderBase = await client.api('/identity/identityProviders/MSASignup-OAUTH')
    .get();

```