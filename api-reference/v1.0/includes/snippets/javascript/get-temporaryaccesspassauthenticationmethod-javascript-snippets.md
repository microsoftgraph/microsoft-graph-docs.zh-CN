---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0630f095e2778d55211d2767c982af6a39b9bfd3
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093170"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let temporaryAccessPassAuthenticationMethod = await client.api('/users/071cc716-8147-4397-a5ba-b2105951cc0b/authentication/temporaryAccessPassMethods/05267842-25b2-4b21-8abd-8e4982796f7f')
    .get();

```