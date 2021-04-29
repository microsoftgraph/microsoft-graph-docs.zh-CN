---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4893ce58e10b1eb055946b1fb6fbe54faa1148cc
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52081536"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProvider = {
  '@odata.id': 'https://graph.microsoft.com/beta/identityProviders/{id}'
};

await client.api('/identity/b2cUserFlows/{id}/identityProviders/$ref')
    .version('beta')
    .post(identityProvider);

```