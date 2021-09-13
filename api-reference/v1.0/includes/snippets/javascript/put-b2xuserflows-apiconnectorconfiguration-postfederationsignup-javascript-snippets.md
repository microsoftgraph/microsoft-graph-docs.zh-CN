---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 757cd25d86e7800830fb7c68df8e41392329cc7eeee45e8a87251684fcef1f79
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105421"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityApiConnector = {
    '@odata.id': 'https://graph.microsoft.com/v1.0/identity/apiConnectors/{id}'   
};

await client.api('/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postFederationSignup/$ref')
    .put(identityApiConnector);

```