---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa0bbb3c24d8a7fe472fe377df4fd8a6595e3d6e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808248"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let windowsHelloForBusinessMethods = await client.api('/users/annie@contoso.com/authentication/windowsHelloForBusinessMethods')
    .version('beta')
    .get();

```