---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c118c1186e2c0157ad1601cc18695231c539abe7803aa579d6b6ea02ee168ba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902535"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const agreement = {
  displayName: 'displayName-value',
  isViewingBeforeAcceptanceRequired: true
};

await client.api('/identityGovernance/termsOfUse/agreements/{id}')
    .version('beta')
    .update(agreement);

```