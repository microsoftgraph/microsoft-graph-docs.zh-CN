---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33486252821ca75046a33f8597a1e5c24f227ae1
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334629"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/places/bldg2@contoso.com/microsoft.graph.roomlist/rooms')
    .get();

```