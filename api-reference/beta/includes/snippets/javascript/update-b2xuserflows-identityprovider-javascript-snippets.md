---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90152ca06ec28fcf147ab79e34110f2c85c739af
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52081588"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProvider = {
  '@odata.id': 'https://graph.microsoft.com/beta/identityProviders/{id}'
};

await client.api('/identity/b2xUserFlows/{id}/identityProviders/$ref')
    .version('beta')
    .post(identityProvider);

```