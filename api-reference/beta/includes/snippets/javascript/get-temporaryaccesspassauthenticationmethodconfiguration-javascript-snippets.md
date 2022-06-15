---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81309b2eb2bdb21dc35b903fc817ceeddf488431
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093526"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let authenticationMethodConfiguration = await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/temporaryAccessPass')
    .version('beta')
    .get();

```