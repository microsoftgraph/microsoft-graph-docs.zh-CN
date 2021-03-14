---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9642e7c3491653511705e00866abbf7c1c53a642
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810191"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProvider = await client.api('/identityProviders/Amazon-OAuth')
    .get();

```