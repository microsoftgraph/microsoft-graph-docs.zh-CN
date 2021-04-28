---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f795e554dd7505defce854f31d9d691a67b00e40
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51919311"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProviders = {
  '@odata.id': 'https://graph.microsoft.com/v1.0/identityProviders/Facebook-OAUTH'
};

await client.api('/identity/b2xUserFlows/B2X_1_Partner/identityProviders/$ref')
    .update(identityProviders);

```