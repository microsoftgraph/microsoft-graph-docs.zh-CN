---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b012180f5ad2f15de98f4d4743ab84fc04cbce0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801349"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let message = await client.api('/me/messages/AAMkADYAAAImV_lAAA=')
    .version('beta')
    .get();

```