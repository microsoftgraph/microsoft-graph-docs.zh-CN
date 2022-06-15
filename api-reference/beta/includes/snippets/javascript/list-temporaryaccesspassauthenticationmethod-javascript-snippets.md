---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7dc4f128662202685933dcabacac238ef73bf945
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098772"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let temporaryAccessPassMethods = await client.api('/users/071cc716-8147-4397-a5ba-b2105951cc0b/authentication/temporaryAccessPassMethods')
    .version('beta')
    .get();

```