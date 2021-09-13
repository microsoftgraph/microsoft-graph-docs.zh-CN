---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 650992f239d5a7c1484169918ab969196bb444ec471bf7f194a904b462d03c56
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158731"
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