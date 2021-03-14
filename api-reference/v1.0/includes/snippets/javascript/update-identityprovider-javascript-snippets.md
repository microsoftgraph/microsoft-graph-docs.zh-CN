---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e1a6d02522d4eb7a36f706b030d10dcdc114c0b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789129"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProvider = {
    clientSecret: '1111111111111'
};

await client.api('/identityProviders/Amazon-OAuth')
    .update(identityProvider);

```