---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f1fa9e89885bcc7bdcd8ad01ef25ca65f1b85f48
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520011"
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
    .post({identityProvider : identityProvider});

```