---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89971dbd84df92c9577988f9c011ab963eea68c5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772497"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getrecentnotebooks = await client.api('/me/onenote/notebooks/getrecentnotebooks(includePersonalNotebooks=true)')
    .get();

```