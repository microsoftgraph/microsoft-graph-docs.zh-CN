---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1a6558eca2374875a0533dedd11708a1cbf9047
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778647"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let search = await client.api('/me/drive/search(q='Contoso Project')')
    .get();

```