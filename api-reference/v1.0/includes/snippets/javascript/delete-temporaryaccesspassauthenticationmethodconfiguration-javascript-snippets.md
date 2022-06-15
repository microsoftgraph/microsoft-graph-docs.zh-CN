---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45fd7f53248c8d31ad8bedfd565e79399e13aab6
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094548"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/temporaryAccessPass`')
    .delete();

```