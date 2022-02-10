---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7f663bd807771739a9bf8f18b1d716fc4a33522
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519533"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let authenticationMethodConfiguration = await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/x509Certificate')
    .version('beta')
    .get();

```