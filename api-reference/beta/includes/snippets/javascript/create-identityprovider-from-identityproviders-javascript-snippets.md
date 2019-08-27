---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1b42d0a7fb9e44d83676d4e3d5aa3f9af958704d
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636483"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProvider = {
    name: "Login with Amazon",
    type: "Amazon",
    clientId: "56433757-cadd-4135-8431-2c9e3fd68ae8",
    clientSecret: "000000000000"
};

let res = await client.api('/identityProviders')
    .version('beta')
    .post(identityProvider);

```