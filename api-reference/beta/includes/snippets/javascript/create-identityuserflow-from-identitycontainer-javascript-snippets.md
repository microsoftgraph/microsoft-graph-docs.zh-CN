---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b8d9ba6e9e9870b1c1d1f8bd5404241dd14226feee12af3da61b1f6d2291732
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162208"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityUserFlow = {
  id: 'Pol1',
  userFlowType: 'signUpOrSignIn',
  userFlowTypeVersion: 1
};

await client.api('/identity/userFlows')
    .version('beta')
    .post(identityUserFlow);

```