---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a289028b2a0c7edee1eeec459ed2d5f1d607f791
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802682"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let certificateBasedAuthConfiguration = await client.api('/organization/{id}/certificateBasedAuthConfiguration')
    .get();

```