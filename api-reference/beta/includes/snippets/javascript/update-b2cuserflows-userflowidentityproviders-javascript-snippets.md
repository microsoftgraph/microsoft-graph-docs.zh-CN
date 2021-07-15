---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90989c1edd2632937554b530582ea5572fe1c673
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439675"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userFlowIdentityProviders = {
  '@odata.id': 'https://graph.microsoft.com/beta/identity/identityProviders/{id}'
};

await client.api('/identity/b2cUserFlows/B2C_test_signin_signup/userflowIdentityProviders/$ref')
    .version('beta')
    .update(userFlowIdentityProviders);

```