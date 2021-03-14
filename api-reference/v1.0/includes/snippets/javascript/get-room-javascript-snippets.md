---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71a5b73926646e9e0fc4b536e21942d23a0f571d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790776"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let place = await client.api('/places/3162F1E1-C4C0-604B-51D8-91DA78989EB1')
    .get();

```