---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a8891890a49fdc5748d162dd425c95821e026cf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807409"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drive = await client.api('/users/{idOrUserPrincipalName}/drive')
    .get();

```