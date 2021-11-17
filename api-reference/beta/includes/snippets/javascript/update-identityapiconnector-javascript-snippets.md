---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da21516483f73c56caeaf685a59912739fe6287f4976f5118d0896ebca278639
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220671"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityApiConnector = {
  authenticationConfiguration: {
    '@odata.type': '#microsoft.graph.pkcs12Certificate',
    pkcs12Value: 'eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA',
    password: 'secret'
  }
};

await client.api('/identity/apiConnectors/{identityApiConnectorId}')
    .version('beta')
    .update(identityApiConnector);

```