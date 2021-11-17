---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5da626b68a3cc1c54c8cd828257f8e1e4d8062b1e3a3f7af66b47ec4fb2e8d4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219498"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const trustFrameworkKey = {
  key: 'Base64-encoded-pfx-content',
  password: 'password-value'
};

await client.api('/trustFramework/keySets/{id}/uploadPkcs12')
    .version('beta')
    .post(trustFrameworkKey);

```