---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdeae770abf3736118226463f860c6163442890a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797862"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let memberOf = await client.api('/contacts/{id}/memberOf')
    .get();

```