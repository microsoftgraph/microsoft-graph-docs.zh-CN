---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4db7bba680a104550187efbf85607e1a8cb5809c
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519571"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/x509Certificate')
    .version('beta')
    .delete();

```