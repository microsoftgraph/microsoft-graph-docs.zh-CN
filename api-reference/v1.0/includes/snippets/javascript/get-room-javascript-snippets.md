---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ea8f6054f82703c9c2f123cc8b881a2caaa7127
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332364"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/places/3162F1E1-C4C0-604B-51D8-91DA78989EB1')
    .get();

```