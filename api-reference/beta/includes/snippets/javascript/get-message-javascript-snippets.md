---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24f5bedb5524a9d2c68acd9da37f44d1c0d858cb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788450"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let message = await client.api('/me/messages/AAMkAGI1AAAoZCfHAAA=')
    .version('beta')
    .get();

```