---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c5322bda59fbeba8076e368616baa4fd90d0bb2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804122"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let owners = await client.api('/groups/{id}/owners')
    .get();

```