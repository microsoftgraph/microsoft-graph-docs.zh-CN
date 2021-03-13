---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b4cddb8a67a5808b1c1960ce6549aaf4c058b43
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788611"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/education/schools/10002/users')
    .version('beta')
    .get();

```