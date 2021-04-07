---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60b9ecd1c5c4d66b059f2f09baf09a7eaa615c1a
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51613507"
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