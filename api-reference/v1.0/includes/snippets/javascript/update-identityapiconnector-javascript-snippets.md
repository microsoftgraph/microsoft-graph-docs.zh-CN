---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da239e568a1627b6f6f49175aaaad5f0f57660a8a856f2aafe936b1aacda854c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219345"
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

await client.api('/identity/apiConnectors/be1f769b-9b13-437e-b540-79a905c4932c')
    .update(identityApiConnector);

```