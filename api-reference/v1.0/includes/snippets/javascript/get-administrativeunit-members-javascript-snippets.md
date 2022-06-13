---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e02127ed605cabc568cbc796eeb5165799f125b
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66040841"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryObject = await client.api('/directory/administrativeUnits/c5729e7c-988e-417b-b287-14f5bd4711d8/members/7c06cd31-7c30-4f3b-a5c3-444cd8dd63ac')
    .get();

```