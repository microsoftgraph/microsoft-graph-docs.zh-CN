---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35d73f96f647d3c118fc4b6eb59243edd65cade683dcbc548e2bf924985c33c9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220313"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/drive/items/{item-id}/content?format=%7Bformat%7D')
    .version('beta')
    .get();

```