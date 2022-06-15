---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c90b4fd6f75212ce5f6d0f271cb057f9b9b5ac89
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094506"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationMethodConfiguration = {
  isUsableOnce: true
};

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/temporaryAccessPass')
    .update(authenticationMethodConfiguration);

```