---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44460cfe2e970584fee0c5efb6f30c1c5e836167
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437741"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationMethodConfiguration = {
   '@odata.type':'#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration',
  isUsableOnce: true
};

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/temporaryAccessPass')
    .update(authenticationMethodConfiguration);

```