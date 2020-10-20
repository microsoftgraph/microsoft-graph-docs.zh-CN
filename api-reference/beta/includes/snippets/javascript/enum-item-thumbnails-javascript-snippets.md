---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e9244f62bf7857aa08c8b53a68bb8d736ef588a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618442"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/thumbnails')
    .version('beta')
    .get();

```