---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e0d0f91fa7d8b36f2e1a1dfd16bb48e7d2b103b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60946248"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedGroupSource = {
  group: {
    mail: 'SecretGroup@contoso.com'
  },
  includedSources: 'mailbox, site'
};

await client.api('/compliance/ediscovery/cases/15d80234-8320-4f10-96d0-d98d53ffdfc9/custodians/8904528fef4d4578b44f71a80188f400/unifiedGroupSources')
    .version('beta')
    .post(unifiedGroupSource);

```