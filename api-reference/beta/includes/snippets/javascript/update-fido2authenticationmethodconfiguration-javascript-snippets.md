---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f150c931babc97247d969372a704e69219a695c3cc035c7f1160d9e923c46c8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218552"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationMethodConfiguration = {
    '@odata.type': '#microsoft.graph.fido2AuthenticationMethodConfiguration',
    state: 'enabled',
    isAttestationEnforced: 'true'
};

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2')
    .version('beta')
    .update(authenticationMethodConfiguration);

```