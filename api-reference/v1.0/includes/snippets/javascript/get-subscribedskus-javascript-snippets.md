---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 374173e2c4c1143bb5d1a14a098b6e45d6fe999b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786951"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let subscribedSkus = await client.api('/subscribedSkus')
    .get();

```