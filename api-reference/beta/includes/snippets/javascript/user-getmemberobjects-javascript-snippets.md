---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 416fbaf3257cea7575e52aa282fa53181dcb861a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804833"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: true
};

await client.api('/me/getMemberObjects')
    .version('beta')
    .post(string);

```