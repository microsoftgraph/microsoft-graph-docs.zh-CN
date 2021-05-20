---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51352ca7e08dab0931d5527d2cafaa6c2bd23e16
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51919228"
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