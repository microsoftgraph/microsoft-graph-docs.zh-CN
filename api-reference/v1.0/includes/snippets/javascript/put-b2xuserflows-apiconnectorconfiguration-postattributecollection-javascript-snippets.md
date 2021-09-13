---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65f4bd7868be34778a1a9802cf4da245b08f3edb7db43a58afd9f24cc1b4f998
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105420"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityApiConnector = {
    '@odata.id': 'https://graph.microsoft.com/v1.0/identity/apiConnectors/{id}'   
};

await client.api('/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref')
    .put(identityApiConnector);

```