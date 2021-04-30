---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea317750508a7b9006b52f19450ac50976fd45b9
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52081543"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProvider = {
  '@odata.id': 'https://graph.microsoft.com/v1.0/identityProviders/Facebook-OAUTH'
};

await client.api('/identity/b2xUserFlows/B2X_1_Partner/identityProviders/$ref')
    .post(identityProvider);

```