---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 956ee5d9491ec646a3f7c2820419e2643d6dd7ea1220b48f9306d18fc4fdf2dd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103920"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const trustFrameworkKey = {
  key: 'key-value'
};

await client.api('/trustFramework/keySets/{id}/uploadCertificate')
    .version('beta')
    .post(trustFrameworkKey);

```